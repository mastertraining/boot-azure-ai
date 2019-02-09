# Azure AI Services Boot Camp

## The Workshop

The Workshop Complimentary for Azure AI Services

## Slides & Video
* [AI made easy on Cloud platform](https://gitpitch.com/tlaothong/ai-cloud/cast)
* [Microsoft AI](slides/MsAi.pdf)
* [Machine Learning (Algorithms Cheat Sheet link)](slides/MLCheatSheetAndBooks.pdf)

## Analyze an image
* [Document](https://docs.microsoft.com/en-us/azure/cognitive-services/Computer-vision/quickstarts-sdk/csharp-analyze-sdk)
* [Source code](https://github.com/Azure-Samples/cognitive-services-vision-csharp-sdk-quickstarts.git)
* (Demo) Path: **ComputerVision/AnalyzeImage**
* (Workshop) Path: **ComputerVision/ExtractText**
* Image Url: https://upload.wikimedia.org/wikipedia/commons/thumb/d/dd/Cursive_Writing_on_Notebook_paper.jpg/800px-Cursive_Writing_on_Notebook_paper.jpg
### Commands
**Package**
```
dotnet add package Microsoft.Azure.CognitiveServices.Vision.ComputerVision
dotnet restore
```

## Image classification
* [Document](https://docs.microsoft.com/en-us/azure/cognitive-services/Custom-Vision-Service/csharp-tutorial)
* [Custom Vision website](https://customvision.ai)
* [Source code](https://github.com/Azure-Samples/cognitive-services-dotnet-sdk-samples.git)
* (Demo) Path: **CustomVision/ImageClassification**
* (Workshop) Path: **CustomVision/ObjectDetection**

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

## Keys
|กลุ่ม|Endpoint|Key|
|--|--|--|
|1|https://southeastasia.api.cognitive.microsoft.com|33a811602f07482eb794e91f2da27885|
|2|https://southeastasia.api.cognitive.microsoft.com|d1bc4ac6adf7455b899b780202ed2413|
|3|https://southeastasia.api.cognitive.microsoft.com|fe5250c045114ccda28d24ec7a96d522|
|4|https://southeastasia.api.cognitive.microsoft.com|bf46109d0b7c4471a4f70add50fd0e24|
|5|https://southeastasia.api.cognitive.microsoft.com|0a55874390de47db9a5e923e065f2fea|
|6|https://southeastasia.api.cognitive.microsoft.com|2061974e1ac844d7a7cad6cbb94450cf|

## Useful links
* [Digital Thailand Club](https://www.facebook.com/digitalthailandclub)
