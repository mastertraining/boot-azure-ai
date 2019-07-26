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
* [Sample image](http://upload.wikimedia.org/wikipedia/commons/3/3c/Shaki_waterfall.jpg)
### Commands
```
dotnet add package Microsoft.Azure.CognitiveServices.Vision.ComputerVision
dotnet restore
```

## 2.Extract handwritten text (Computer Vision)
* [Document](https://docs.microsoft.com/en-us/azure/cognitive-services/Computer-vision/quickstarts-sdk/csharp-hand-text-sdk)
* [Source code](https://raw.githubusercontent.com/mastertraining/boot-azure-ai/master/src/ExtractText/Program.cs)
![img](https://upload.wikimedia.org/wikipedia/commons/thumb/d/dd/Cursive_Writing_on_Notebook_paper.jpg/800px-Cursive_Writing_on_Notebook_paper.jpg)
### Commands
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
```
dotnet add package Microsoft.Azure.CognitiveServices.Vision.CustomVision.Training
dotnet add package Microsoft.Azure.CognitiveServices.Vision.CustomVision.Prediction
dotnet restore
```

## 5.Recognize intents from speech
* [Document](https://docs.microsoft.com/en-us/azure/cognitive-services/speech-service/how-to-recognize-intents-from-speech-csharp)
* [LUIS portal](https://www.luis.ai/home)
* [LUIS get started](https://docs.microsoft.com/en-us/azure/cognitive-services/luis/luis-get-started-create-app)
* [Source code](https://raw.githubusercontent.com/mastertraining/boot-azure-ai/master/RecognizeIntentsFromSpeech.cs)
### Commands
```
dotnet add package Microsoft.CognitiveServices.Speech
dotnet restore
```

## 6.Create and deploy a basic bot
* [Document](https://docs.microsoft.com/en-us/azure/bot-service/bot-builder-tutorial-basic-deploy?view=azure-bot-service-4.0&tabs=csharp%2Cnewrg)
* [Tunneling (ngrok)](https://github.com/Microsoft/BotFramework-Emulator/wiki/Tunneling-(ngrok))
### Commands
```
dotnet publish
```

## 7.Use a Web App Bot enabled with Language Understanding in C#
* [Document](https://docs.microsoft.com/en-us/azure/cognitive-services/luis/luis-csharp-tutorial-bf-v4)

## 8.Run a Spark job on Azure Databricks using the Azure portal
* [Document](https://docs.microsoft.com/en-us/azure/azure-databricks/quickstart-create-databricks-workspace-portal)

## 9.Sentiment analysis on streaming data using Azure Databricks
* [Document](https://docs.microsoft.com/en-us/azure/azure-databricks/databricks-sentiment-analysis-cognitive-services)


## Tools
* [.NET Core](https://dotnet.microsoft.com/download)
* [Visual Studio Code](https://code.visualstudio.com)
* [Bot Framework SDK v4 template for C#](https://marketplace.visualstudio.com/items?itemName=BotBuilder.botbuilderv4)
* [Bot Framework Emulator](https://github.com/microsoft/BotFramework-Emulator/releases)
* [ngrok](https://ngrok.com/download)

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
