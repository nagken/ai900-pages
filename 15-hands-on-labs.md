# Hands-on Labs

> All labs run on a free Microsoft Learn sandbox or your own Azure free account. Each lab takes 15-45 minutes.

## How to start

- Use the **[Microsoft Learn sandbox](https://learn.microsoft.com/training/support/microsoft-learn-sandbox)** built into the modules - no credit card.
- Or get **[$200 free Azure credit](https://azure.microsoft.com/free/)** for your own subscription.
- Or use the **F0 (free) tier** of most Azure AI services (5K transactions / month).

## Lab 1 - Provision and call a multi-service Azure AI services resource

- Module: [Get started with Azure AI services](https://learn.microsoft.com/training/modules/get-started-azure-ai/)
- You will: create a multi-service resource in the portal, copy endpoint + key, then make a REST call to the Language API.
- Why it matters: you must recognize **endpoint + key auth** vs **Microsoft Entra (Azure AD) auth** and the trade-offs.

## Lab 2 - Image Analysis 4.0

- Module: [Analyze images with Azure AI Vision](https://learn.microsoft.com/training/modules/analyze-images/)
- You will: upload images, run tags / caption / dense captions / objects / read.
- Why: cement Image Analysis vs Read vs Custom Vision differences.

## Lab 3 - Custom Vision

- Module: [Classify images with Custom Vision](https://learn.microsoft.com/training/modules/classify-images-custom-vision/)
- You will: upload labeled images, train iterations, evaluate, publish, score.
- Why: only way to internalize the **classification vs detection** project type and **iteration / publish** workflow.

## Lab 4 - Document Intelligence prebuilt receipts

- Module: [Analyze receipts with the Document Intelligence service](https://learn.microsoft.com/training/modules/analyze-receipts-form-recognizer/)
- You will: send receipt images to the prebuilt-receipt model and inspect extracted fields.
- Why: confirms the prebuilt -> fields contract and how confidence scores work.

## Lab 5 - Sentiment + key phrases + entities

- Module: [Fundamentals of Text Analysis with the Language Service](https://learn.microsoft.com/training/modules/analyze-text-with-text-analytics-service/)
- You will: call Language API with sample text and see all four built-in features at once.
- Why: drills the prebuilt-feature catalog you must memorize.

## Lab 6 - Build a CLU intent model

- Module: [Build a conversational language understanding model](https://learn.microsoft.com/training/modules/create-language-understanding-model/)
- You will: define intents + entities, label utterances, train, deploy, predict.
- Why: makes the **intent vs entity** distinction concrete (vs Custom Question Answering).

## Lab 7 - Custom Question Answering bot

- Module: [Create a question answering solution](https://learn.microsoft.com/training/modules/create-question-answer-solution-ai-language/)
- You will: ingest a FAQ page, edit pairs, deploy, query.
- Why: shows when CQA is right vs CLU.

## Lab 8 - Speech to Text + Text to Speech

- Module: [Recognize and synthesize speech](https://learn.microsoft.com/training/modules/recognize-synthesize-speech/)
- You will: transcribe a recording, then synthesize a sentence in two neural voices.
- Why: forces you to use **Speech Studio**, where most Limited Access features are surfaced.

## Lab 9 - Translation pipeline

- Module: [Translate text with the Translation service](https://learn.microsoft.com/training/modules/translate-text-with-translation-service/)
- You will: translate strings + auto-detect language, then try transliteration.
- Why: clarifies Text vs Document vs Custom Translator boundaries.

## Lab 10 - Train an AutoML classification model

- Module: [Use Automated ML in Azure ML](https://learn.microsoft.com/training/modules/use-automated-machine-learning/)
- You will: upload a CSV, run AutoML, deploy winner.
- Why: makes the Azure ML workspace + compute + endpoint loop tangible.

## Lab 11 - Designer pipeline

- Module: [Create a regression model with Designer](https://learn.microsoft.com/training/modules/create-regression-model-azure-machine-learning-designer/)
- You will: drag-drop import -> split -> train -> score -> evaluate components.
- Why: visualizes the lifecycle without writing Python.

## Lab 12 - Generative AI playground (Foundry / OpenAI)

- Module: [Get started with Azure OpenAI Service](https://learn.microsoft.com/training/modules/explore-azure-openai/)
- You will: deploy GPT-4o, chat in the playground, change system message + temperature.
- Why: the only way to *feel* prompt engineering effects.

## Lab 13 - RAG over your own data

- Module: [Implement Retrieval Augmented Generation (RAG) with Azure OpenAI](https://learn.microsoft.com/training/modules/use-own-data-azure-openai/)
- You will: use **Foundry "Add your data"** to point a chat model at a Blob container + Azure AI Search.
- Why: cements the canonical Gen-AI architecture you'll see on the test.

## Lab 14 - Content Safety + Prompt Shields

- Module: [Fundamentals of Responsible Generative AI](https://learn.microsoft.com/training/modules/responsible-generative-ai/)
- You will: post benign + harmful + jailbreak prompts in the Content Safety Studio and watch each filter fire.
- Why: ties the four harm categories + Prompt Shields together.

## Lab 15 - Build a no-code Copilot Studio bot

- Module: [Get started with Microsoft Copilot Studio](https://learn.microsoft.com/training/paths/get-started-microsoft-copilot-studio/)
- You will: build a topic-driven copilot, connect to a knowledge source.
- Why: rounds out the Gen-AI "low-code" answer pattern.

---

[<- Pitfalls](14-pitfalls.md) - [Architecture Center ->](16-architecture-center.md)
