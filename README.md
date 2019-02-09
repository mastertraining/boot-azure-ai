# Azure AI Services Boot Camp

## The Workshop

The Workshop Complimentary for Azure AI Services



## [Analyze an image](https://docs.microsoft.com/en-us/azure/cognitive-services/Computer-vision/quickstarts-sdk/csharp-analyze-sdk)
* [Source code](https://github.com/Azure-Samples/cognitive-services-vision-csharp-sdk-quickstarts.git)
* (Demo) Path: **ComputerVision/AnalyzeImage**
* (Workshop) Path: **ComputerVision/ExtractText**

## [Image classification](https://docs.microsoft.com/en-us/azure/cognitive-services/Custom-Vision-Service/csharp-tutorial)
* [Custom Vision website](https://customvision.ai)
* [Source code](https://github.com/Azure-Samples/cognitive-services-dotnet-sdk-samples.git)
* (Demo) Path: **CustomVision/ImageClassification**
* (Workshop) Path: **CustomVision/ObjectDetection**

## [Recognize intents from speech](https://docs.microsoft.com/en-us/azure/cognitive-services/speech-service/how-to-recognize-intents-from-speech-csharp)
* [LUIS portal](https://www.luis.ai/home)
```
using System;
using System.Threading.Tasks;
using Microsoft.CognitiveServices.Speech;
using Microsoft.CognitiveServices.Speech.Audio;
using Microsoft.CognitiveServices.Speech.Intent;

namespace demoluis
{
    class Program
    {
        static void Main(string[] args)
        {
            RecognizeIntentAsync().Wait();
            Console.WriteLine("Please press Enter to continue.");
            Console.ReadLine();
        }

        static async Task RecognizeIntentAsync()
        {
            // Creates an instance of a speech config with specified subscription key
            // and service region. Note that in contrast to other services supported by
            // the Cognitive Services Speech SDK, the Language Understanding service
            // requires a specific subscription key from https://www.luis.ai/.
            // The Language Understanding service calls the required key 'endpoint key'.
            // Once you've obtained it, replace with below with your own Language Understanding subscription key
            // and service region (e.g., "westus").
            // The default language is "en-us".
            var config = SpeechConfig.FromSubscription("YourLanguageUnderstandingSubscriptionKey", "YourLanguageUnderstandingServiceRegion");

            // Creates an intent recognizer using microphone as audio input.
            using (var recognizer = new IntentRecognizer(config))
            {
                // Creates a Language Understanding model using the app id, and adds specific intents from your model
                var model = LanguageUnderstandingModel.FromAppId("YourLanguageUnderstandingAppId");
                recognizer.AddIntent(model, "HomeAutomation.TurnOff", "off");
                recognizer.AddIntent(model, "HomeAutomation.TurnOn", "on");

                // Starts recognizing.
                Console.WriteLine("Say something...");

                // Performs recognition. RecognizeOnceAsync() returns when the first utterance has been recognized,
                // so it is suitable only for single shot recognition like command or query. For long-running
                // recognition, use StartContinuousRecognitionAsync() instead.
                var result = await recognizer.RecognizeOnceAsync().ConfigureAwait(false);

                // Checks result.
                if (result.Reason == ResultReason.RecognizedIntent)
                {
                    Console.WriteLine($"RECOGNIZED: Text={result.Text}");
                    Console.WriteLine($"    Intent Id: {result.IntentId}.");
                    Console.WriteLine($"    Language Understanding JSON: {result.Properties.GetProperty(PropertyId.LanguageUnderstandingServiceResponse_JsonResult)}.");
                }
                else if (result.Reason == ResultReason.RecognizedSpeech)
                {
                    Console.WriteLine($"RECOGNIZED: Text={result.Text}");
                    Console.WriteLine($"    Intent not recognized.");
                }
                else if (result.Reason == ResultReason.NoMatch)
                {
                    Console.WriteLine($"NOMATCH: Speech could not be recognized.");
                }
                else if (result.Reason == ResultReason.Canceled)
                {
                    var cancellation = CancellationDetails.FromResult(result);
                    Console.WriteLine($"CANCELED: Reason={cancellation.Reason}");

                    if (cancellation.Reason == CancellationReason.Error)
                    {
                        Console.WriteLine($"CANCELED: ErrorCode={cancellation.ErrorCode}");
                        Console.WriteLine($"CANCELED: ErrorDetails={cancellation.ErrorDetails}");
                        Console.WriteLine($"CANCELED: Did you update the subscription info?");
                    }
                }
            }
        }
    }
}
```
