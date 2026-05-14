# AI-900 Glossary

> Alphabetical, exam-focused. If a term is *also* a renamed service, the old name is in parentheses.

| Term | Definition |
|---|---|
| **Abstractive summarization** | Generates a fresh summary in new wording. |
| **Accuracy** | Fraction of correct predictions. Misleading on imbalanced data. |
| **Agent** | LLM-driven program that plans + uses tools to complete multi-step goals. |
| **Anomaly detection** | Identify outliers / unusual events. |
| **AUC (Area Under ROC Curve)** | Classifier separability metric; 1.0 = perfect, 0.5 = random. |
| **Automated ML (AutoML)** | Azure ML feature that iterates algorithms + featurization to find the best model. |
| **Azure AI Document Intelligence** *(was Form Recognizer)* | Extract structured fields from forms (prebuilt + custom). |
| **Azure AI Foundry** *(was AI Studio)* | Unified portal for Gen-AI: hub, project, model catalog, playgrounds, evaluations. |
| **Azure AI Language** | Text analytics + CLU + Custom Question Answering. |
| **Azure AI Search** *(was Cognitive Search)* | Search platform with vector + keyword + skillset enrichment. |
| **Azure AI services** *(was Cognitive Services)* | Family of prebuilt AI APIs (Vision, Language, Speech, Translator, Document Intelligence). |
| **Azure AI Speech** | STT + TTS + Speech Translation + Speaker Recognition. |
| **Azure AI Translator** | Text + document + custom translation. |
| **Azure AI Vision** *(was Computer Vision)* | Image Analysis 4.0 + Read OCR + Spatial Analysis. |
| **Azure ML Designer** | Drag-drop visual ML pipelines (no-code). |
| **Azure OpenAI Service** | OpenAI models (GPT, DALL-E, Whisper, embeddings) hosted on Azure. |
| **Batch endpoint** | Azure ML endpoint for async scoring of large datasets. |
| **Caption** | Whole-image one-sentence description (Image Analysis). |
| **Classification** | Predict a category. Binary or multi-class. |
| **Clustering** | Group similar items without labels. |
| **CLU (Conversational Language Understanding)** *(was LUIS)* | Predict intent + entities from utterance. |
| **Compute cluster** | Autoscaling Azure ML compute for training. |
| **Compute instance** | Single-VM dev environment in Azure ML. |
| **Confusion matrix** | TP / FP / TN / FN table for classifier evaluation. |
| **Content Safety** | Azure service that filters Hate / Sexual / Violence / Self-harm + Prompt Shields + Groundedness. |
| **Context window** | Max tokens an LLM can read in one call. |
| **Custom Neural Voice** | Train a brand-specific TTS voice (Limited Access). |
| **Custom Question Answering** *(was QnA Maker)* | FAQ KB question matching. |
| **Custom Vision** | Train your own image classification / object detection. |
| **DALL-E** | Image generation model in Azure OpenAI. |
| **Deep learning** | Neural networks with many layers. |
| **Dense captions** | Captions per image region. |
| **Embedding** | Vector representing meaning of text or images. |
| **Endpoint** | Deployed model accessible via API. Real-time or batch. |
| **Entity** | Named concept (Person, Org, Location, Date, ...) extracted from text. |
| **Extractive summarization** | Picks existing sentences as the summary. |
| **F1 score** | Harmonic mean of precision and recall. |
| **Face (Azure AI Face)** | Detect / verify / identify faces (identification = Limited Access). |
| **Feature** | Input column. |
| **Few-shot prompting** | Include 1+ example IO pairs in the prompt. |
| **Fine-tuning** | Update a model's weights with your training pairs to change behavior / style. |
| **Foundation model** | Large pretrained model adaptable to many tasks. |
| **Function calling** | LLM invokes a defined function/tool with structured arguments. |
| **GPT-4o** | OpenAI's flagship multimodal model (text + vision + audio). |
| **Groundedness** | Whether an answer is supported by retrieved source data. |
| **Hallucination** | LLM inventing facts confidently. |
| **Hub (in Foundry)** | Shared workspace with connections, compute, content safety. |
| **Hyperparameter** | Tunable model setting (learning rate, depth). |
| **Image Analysis 4.0** | Prebuilt image features (tags, captions, objects, dense captions, smart crops). |
| **Image classification** | Predict whole-image label. |
| **Inference** | Running a trained model on new data. |
| **Intent** | What the user wants to do, predicted by CLU. |
| **Knowledge mining** | Pattern of extracting structure from unstructured data using Azure AI Search + skillsets. |
| **Label** | Target column the model predicts. |
| **Language detection** | Identify the language of text. |
| **Limited Access** | Microsoft-gated services (Face Identification, Custom Neural Voice, Liveness). |
| **LLM (Large Language Model)** | Foundation model focused on text. |
| **MAE (Mean Absolute Error)** | Regression metric - average error magnitude. |
| **Microsoft Copilot Studio** | Low-code platform for custom copilots. |
| **MLOps** | DevOps practices for ML - versioning, CI/CD, monitoring, retraining. |
| **Model registry** | Versioned store for trained models. |
| **NER (Named Entity Recognition)** | Extract entities (people, places, orgs, ...). |
| **Object detection** | Bounding boxes + labels per object. |
| **OCR (Optical Character Recognition)** | Read text in images. |
| **Opinion mining** | Aspect-level sentiment ("food positive, service negative"). |
| **Overfitting** | Model memorizes training; fails on new data. |
| **PII detection** | Identify / redact personal information. |
| **Pipeline (Azure ML)** | Multi-step ML graph (prep -> train -> register -> deploy). |
| **Precision** | Of items predicted positive, fraction actually positive. |
| **Prebuilt model** | Ready-to-use model - no training required. |
| **Project (in Foundry)** | Working folder inside a hub for a specific app. |
| **Prompt** | Input text sent to an LLM. |
| **Prompt engineering** | Crafting prompts (system message, instructions, examples) to steer model behavior. |
| **Prompt flow** | Visual editor in Foundry for LLM app pipelines. |
| **Prompt Shields** | Content Safety feature blocking jailbreak / injection. |
| **Provisioned Throughput Units (PTUs)** | Reserved capacity SKU for Azure OpenAI. |
| **R^2** | Regression metric - fraction of variance explained. |
| **RAG (Retrieval Augmented Generation)** | Inject retrieved docs into the prompt to ground answers. |
| **Read API** | OCR feature in Azure AI Vision (and Document Intelligence). |
| **Real-time endpoint** | Low-latency online endpoint for single requests. |
| **Recall (sensitivity)** | Of actual positives, fraction caught. |
| **Regression** | Predict a numeric value. |
| **Reinforcement learning** | Learn via reward signal. |
| **Responsible AI** | Six Microsoft principles: Fairness, Reliability/Safety, Privacy/Security, Inclusiveness, Transparency, Accountability. |
| **RMSE** | Regression metric - penalizes big errors more. |
| **Sentiment analysis** | Classify text as positive / neutral / negative. |
| **Speech to Text (STT)** | Transcribe audio to text. |
| **Speech Translation** | Translate spoken audio between languages. |
| **Speaker Recognition** | Verify or identify by voice. |
| **Supervised learning** | Train with labeled data. |
| **System message** | Hidden instruction setting LLM persona / rules. |
| **Tag (image)** | Single-word descriptor of image content. |
| **Temperature** | LLM randomness 0-2. |
| **Text to Speech (TTS)** | Synthesize speech from text. |
| **Token** | Chunk of text the model processes. Pricing unit. |
| **Top-p** | Sample from top-probability mass; alternate to temperature. |
| **Transformer** | Attention-based architecture powering modern LLMs. |
| **Underfitting** | Model is too simple to capture patterns. |
| **Unsupervised learning** | Train without labels (clustering, anomaly). |
| **Validation set** | Subset of data used during training to tune hyperparameters. |
| **Video Indexer** | Auto-extract insights (faces, OCR, sentiment, topics) from video. |
| **Whisper** | OpenAI speech-to-text model in Azure OpenAI. |
| **Workspace (Azure ML)** | Top-level container for ML assets, runs, and models. |
| **Zero-shot prompting** | Prompt with instruction only, no examples. |

---

[<- Microsoft Resources](11-microsoft-resources.md) - [Flashcards ->](13-flashcards.md)
