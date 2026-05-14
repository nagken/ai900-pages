# AI-900 Exam Decision Reference (Cheatsheet)

> Single-page "when X then Y" lookup. Print this. Skim 60 minutes before the test.

## AI workload classifier

| Question wording | Workload |
|---|---|
| "describe / tag / detect / read / faces / OCR" | **Computer vision** |
| "translate / summarize / sentiment / entities / chatbot intent / FAQ bot" | **Natural language processing** |
| "generate text / image / chat / RAG / fine-tune / Foundry / OpenAI" | **Generative AI** |
| "predict number / category / cluster / classify with my labels" | **Machine learning** |
| "find anomaly / outlier / unusual" | **Anomaly detection** (ML) |
| "knowledge mining over millions of docs" | **AI search / Knowledge Mining** |

## Azure AI service map

| Want | Pick |
|---|---|
| Tag / caption / OCR an image | **Azure AI Vision (Image Analysis 4.0 / Read)** |
| Train your own image classifier | **Custom Vision** |
| Detect / verify / identify a face | **Azure AI Face** (Identification = Limited Access) |
| Insights from a video | **Azure Video Indexer** |
| Extract fields from invoice / receipt / ID | **Azure AI Document Intelligence** (prebuilt models) |
| Plain-text translation | **Azure AI Translator - Text Translation** |
| Translate a Word doc keeping format | **Azure AI Translator - Document Translation** |
| Speech-to-text or text-to-speech | **Azure AI Speech** |
| Speech-to-speech translation | **Azure AI Speech - Speech Translation** |
| Brand voice for IVR | **Custom Neural Voice** (Limited Access) |
| Sentiment / entities / key phrases / PII / summarize | **Azure AI Language** (prebuilt) |
| Chatbot that recognizes intents and slots | **Conversational Language Understanding (CLU)** |
| Bot that answers from FAQ docs | **Custom Question Answering** |
| Generative AI chat / RAG / model catalog | **Azure AI Foundry + Azure OpenAI** |
| Block hate / sexual / violence / jailbreak | **Azure AI Content Safety** (with **Prompt Shields**) |
| Low-code custom copilot for HR | **Microsoft Copilot Studio** |
| Train any classic ML model | **Azure Machine Learning** |

## ML problem-type cheat

| Wording | Pick |
|---|---|
| "predict price / demand / temperature" (number) | **Regression** |
| "spam vs ham, fraud vs not" (category) | **Classification** |
| "group customers without labels" | **Clustering** |
| "fraud / defect outliers" | **Anomaly detection** |
| "recommend a product" | **Recommendation** (matrix factorization, deep learning) |

## Responsible AI quick map

| Principle | Hint phrase |
|---|---|
| **Fairness** | "no bias across gender / race / region" |
| **Reliability & safety** | "consistent under stress, fails safely" |
| **Privacy & security** | "PII, encryption, customer data control" |
| **Inclusiveness** | "accessible to all, alt text, captions" |
| **Transparency** | "explainability, interpretability, model card" |
| **Accountability** | "governance, audit, ownership" |

## Generative AI building-block cheat

| Need | Pick |
|---|---|
| Use latest internal data | **RAG** (Foundry + Azure AI Search + OpenAI) |
| Always answer in a specific style | **Fine-tuning** |
| Tighter behavior, no extra data | **Prompt engineering** (system message + few-shot) |
| LLM must call APIs / DB | **Function calling / tools** |
| Multi-step plan: search -> summarize -> email | **Agents** |
| Block prompt injection | **Prompt Shields** |
| Block hallucinations on policy QA | **RAG + Groundedness detection** |

## Service vs feature traps

- **Image Analysis != Custom Vision** (prebuilt vs your labels).
- **Document Intelligence "Read" != AI Vision "Read"** - same name, different services. DI for forms; Vision for general OCR.
- **CLU replaces LUIS.** **Custom Question Answering replaces QnA Maker.**
- **Speech Translation lives in Speech**, not Translator.
- **Foundry replaced AI Studio**; access OpenAI through Foundry.
- **Face attributes (age, emotion, gender) = retired.** Don't pick.
- **Face Identification + Custom Neural Voice = Limited Access.**

## 60-second pre-exam reset

1. Read the question once. Underline the verb (predict, classify, generate, translate, read).
2. Map verb -> workload (CV / NLP / Gen AI / ML).
3. Map workload -> service (Vision / Language / Speech / Translator / Foundry / OpenAI / ML).
4. Map service -> specific feature (Read / Custom / Detect / RAG / etc.).
5. If two services fit, pick the **most specific prebuilt** one that matches the wording.

---

[<- Generative AI](05-generative-ai.md) - [References ->](06-references.md)
