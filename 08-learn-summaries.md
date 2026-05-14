# Microsoft Learn - Module Summaries

> One-paragraph summaries of the official AI-900 learning path modules. Use these as quick refreshers without leaving the study guide.

## Path: Microsoft Azure AI Fundamentals (AI-900T00)

The official AI-900 path bundles five learning paths matching the five exam domains. Each path is free and includes hands-on sandbox labs that use a Microsoft-provided Azure subscription.

---

## 1. Get started with artificial intelligence

- **Fundamentals of AI**: Defines AI workloads (machine learning, computer vision, NLP, document intelligence, knowledge mining, generative AI). Introduces Microsoft Responsible AI principles and the Azure AI portfolio (Azure AI services, Azure AI Foundry, Azure Machine Learning).
- **Fundamentals of Azure AI services**: Walks through provisioning a multi-service or single-service Azure AI services resource, the role of endpoint and key authentication, and using Microsoft Entra (Azure AD) authentication for production.

## 2. Fundamentals of machine learning

- **Fundamentals of machine learning**: Concept-only introduction to supervised vs unsupervised, regression vs classification vs clustering, and key metrics (MAE, RMSE, R^2, accuracy, precision, recall, F1, AUC).
- **Fundamentals of Azure Machine Learning**: Tour of the Azure ML workspace - datastores, datasets, compute, environments, jobs, models, endpoints, pipelines.
- **Use Automated ML in Azure ML**: Walk through running an AutoML experiment from a CSV file, picking task type and primary metric, then deploying the winning model to a real-time endpoint.

## 3. Computer vision

- **Fundamentals of computer vision**: Difference between classification, object detection, OCR, facial detection. Convolutional neural networks (CNNs) explained at concept level.
- **Analyze images with Azure AI Vision**: Image Analysis 4.0 features - tags, captions, dense captions, objects, smart crops, background removal.
- **Read text with Azure AI Vision**: The Read API for printed and handwritten OCR; difference between sync and async modes.
- **Detect, analyze, and recognize faces**: Azure AI Face - detection (open access) vs verification and identification (Limited Access). Note that emotion / gender / age attributes were retired.
- **Analyze receipts with Document Intelligence**: Prebuilt receipt model and what fields it extracts. Custom models for company-specific forms.

## 4. Natural language processing

- **Fundamentals of text analysis with the Language service**: Sentiment, key phrases, entities, language detection, PII, summarization. All prebuilt - no training required.
- **Fundamentals of question answering with the Language service**: Build a knowledge-base bot with **Custom Question Answering** (replaces QnA Maker).
- **Fundamentals of conversational language understanding**: Build a CLU project with intents + entities (replaces LUIS).
- **Fundamentals of Azure AI Speech**: Speech-to-Text (real-time + batch + custom), Text-to-Speech with neural voices, Speech Translation, Speaker Recognition.
- **Fundamentals of language translation**: Text Translation, Document Translation, Custom Translator.

## 5. Generative AI

- **Foundations of generative AI**: What an LLM is, tokens, prompts, completions, embeddings, transformers at a conceptual level.
- **Fundamentals of Azure OpenAI Service**: GPT family for text, DALL-E for images, Whisper for speech, embedding models. PayGo and Provisioned Throughput.
- **Plan and prepare to develop AI solutions on Azure**: Azure AI Foundry hub + project, model catalog, playgrounds, deployments.
- **Fundamentals of Responsible Generative AI**: Identify, measure, mitigate, operate. Content Safety filters (Hate, Sexual, Violence, Self-harm), Prompt Shields, Groundedness.
- **Get started with Microsoft Copilot Studio**: Low-code custom copilots for organizations.

---

## How to read these for the exam

1. Skim each module summary. If anything is unfamiliar, do the full Microsoft Learn module (free).
2. Pay extra attention to **service-vs-feature** distinctions (e.g., Custom Vision vs Image Analysis, CLU vs Custom Question Answering).
3. Memorize the **Limited Access** services: Face Identification, Custom Neural Voice.
4. Memorize the **renamed** services: Document Intelligence (was Form Recognizer), CLU (was LUIS), Custom Question Answering (was QnA Maker), Foundry (was AI Studio).

---

[<- Extra Concepts](07-extra-ai900-concepts.md) - [Reference Architectures ->](09-arch-ai900.md)
