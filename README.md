# Azure AI Services Boot Camp

## The Workshop

The Workshop Complimentary for Azure AI Services

## Slides & Video
* [AI made easy on Cloud platform](https://gitpitch.com/tlaothong/ai-cloud/cast)
* [Microsoft AI](slides/MsAi.pdf)
* [Machine Learning (Algorithms Cheat Sheet link)](slides/MLCheatSheetAndBooks.pdf)
* [Cognitive services repository](https://github.com/Azure-Samples/cognitive-services-vision-csharp-sdk-quickstarts)

## 1.Analyze an image (Computer Vision)
* [Document](https://docs.microsoft.com/en-us/azure/cognitive-services/Computer-vision/quickstarts-sdk/csharp-analyze-sdk)
* [Source code](https://raw.githubusercontent.com/Azure-Samples/cognitive-services-vision-csharp-sdk-quickstarts/master/ComputerVision/AnalyzeImage/Program.cs)
### Commands
**Package**
```
dotnet add package Microsoft.Azure.CognitiveServices.Vision.ComputerVision
dotnet restore
```

## 2.Extract handwritten text (Computer Vision)
* [Document](https://docs.microsoft.com/en-us/azure/cognitive-services/Computer-vision/quickstarts-sdk/csharp-hand-text-sdk)
* [Source code](https://raw.githubusercontent.com/Azure-Samples/cognitive-services-vision-csharp-sdk-quickstarts/master/ComputerVision/ExtractText/Program.cs)
* Image Url: https://upload.wikimedia.org/wikipedia/commons/thumb/d/dd/Cursive_Writing_on_Notebook_paper.jpg/800px-Cursive_Writing_on_Notebook_paper.jpg
### Commands
**Package**
```
dotnet add package Microsoft.Azure.CognitiveServices.Vision.ComputerVision
dotnet restore
```

## 3.Image classification (Custom Vision)
* [Document](https://docs.microsoft.com/en-us/azure/cognitive-services/Custom-Vision-Service/csharp-tutorial)
* [Custom Vision website](https://customvision.ai)
* [Source code](https://github.com/Azure-Samples/cognitive-services-dotnet-sdk-samples.git) 
* Path: **CustomVision/ImageClassification**

### Commands
**Package**
```
dotnet add package Microsoft.Azure.CognitiveServices.Vision.CustomVision.Training
dotnet add package Microsoft.Azure.CognitiveServices.Vision.CustomVision.Prediction
dotnet restore
```

## 4.Object detection (Custom Vision)
* [Document](https://docs.microsoft.com/en-us/azure/cognitive-services/Custom-Vision-Service/csharp-tutorial)
* [Custom Vision website](https://customvision.ai)
* [Source code](https://github.com/Azure-Samples/cognitive-services-dotnet-sdk-samples.git) 
* Path: **CustomVision/ObjectDetection**

### Commands
**Package**
```
dotnet add package Microsoft.Azure.CognitiveServices.Vision.CustomVision.Training
dotnet add package Microsoft.Azure.CognitiveServices.Vision.CustomVision.Prediction
dotnet restore
```

## Recognize intents from speech
* [Document](https://docs.microsoft.com/en-us/azure/cognitive-services/speech-service/how-to-recognize-intents-from-speech-csharp)
* [LUIS portal](https://www.luis.ai/home)
* [Source code](https://github.com/Azure-Samples/cognitive-services-speech-sdk.git)
* (Demo) Path: **samples\csharp\sharedcontent\console\intent_recognition_samples.cs**
### Commands
**Package**
```
dotnet add package Microsoft.CognitiveServices.Speech
dotnet restore
```

## Tools
* [.NET Core](https://dotnet.microsoft.com/download)
* [Visual Studio Code](https://code.visualstudio.com)

## .NET Commands
**Create project**
```
dotnet new console -n YOUR_PROJECT_NAME_HERE
```
**Run**
```
dotnet run
```

## Useful links
* [Digital Thailand Club](https://www.facebook.com/digitalthailandclub)
* [Microsoft Azure pass](https://www.microsoftazurepass.com/)
