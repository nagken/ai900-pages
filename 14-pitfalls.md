# Top Pitfalls (Don't Lose Easy Points)

> Repeated traps from AI-900 retired items, official practice assessment, and Microsoft Learn modules. Skim morning of exam.

## 1. Old service names

| Old name (still on the exam as a distractor) | Pick instead |
|---|---|
| Form Recognizer | **Azure AI Document Intelligence** |
| Cognitive Services | **Azure AI services** |
| Computer Vision | **Azure AI Vision** |
| LUIS | **Conversational Language Understanding (CLU)** |
| QnA Maker | **Custom Question Answering** |
| Translator Text | **Azure AI Translator - Text Translation** |
| Speech Services | **Azure AI Speech** |
| Cognitive Search | **Azure AI Search** |
| AI Studio | **Azure AI Foundry** |

## 2. Service vs feature confusion

- **Image Analysis vs Custom Vision**: prebuilt categories vs your own labels.
- **AI Vision Read vs Document Intelligence Read**: both do OCR, but Document Intelligence is the answer when fields like merchant / total / vendor are wanted.
- **AI Vision (Image Analysis) vs Face**: faces with identity -> Face. Generic image tagging -> Image Analysis.
- **CLU vs Custom Question Answering**: CLU = predict an *intent* + slots. CQA = match a *question* to a stored answer.
- **Translator vs Speech Translation**: text/files -> Translator. Audio -> Azure AI Speech.

## 3. Retired or limited-access features

- **Face attributes (age, gender, emotion, smile, hair)** were retired in 2022. Don't pick.
- **Anomaly Detector** standalone service was retired. Use **Azure ML** or **Stream Analytics**.
- **Personalizer** was retired.
- **Face Identification, Face Liveness, Custom Neural Voice** are **Limited Access** - require Microsoft approval.

## 4. ML metric traps

- **Accuracy** is a trap on imbalanced data. Pick **precision**, **recall**, or **F1**.
- **R^2 closer to 1** is better; **MAE / RMSE lower** is better. Don't reverse them.
- **Confusion matrix** rows/columns differ across vendors - read carefully.

## 5. Generative AI traps

- **Hallucinations** are not solved by "more data" - solve with **RAG + Groundedness detection**.
- **Prompt Shields != Content Safety filters**. Shields = injection / jailbreak. Filters = harm categories.
- **Fine-tuning != RAG**. Fine-tune changes the model's *style/behavior*. RAG injects *current data*.
- **Tokens are billed both ways** - input AND output tokens.
- **Custom Neural Voice is Limited Access**. Standard neural voices are not.
- **Foundry replaced AI Studio.** New name on the test.

## 6. Document Intelligence specifics

- **Prebuilt-Receipt** extracts merchant + line items + total. Plain Read API does not.
- **Layout** model = text + tables + selection marks. Use it when "preserve table structure" is mentioned.
- **Custom model** needs only **5+ labeled samples** for a basic form.

## 7. Speech specifics

- **Real-time STT** for live captions. **Batch STT** for recorded files.
- **Custom Speech** = train the recognizer on your jargon / accents.
- **Custom Neural Voice** = train a *speaker* voice.
- **Speaker Recognition** is voice biometrics - verify (1:1) or identify (1:N).

## 8. Translator specifics

- **Text Translation API** - strings.
- **Document Translation** - preserves DOCX/PPTX/PDF formatting.
- **Custom Translator** - domain-tuned model **called via Text Translation API** (not a separate API surface).
- **Transliteration** != **Translation**. Transliteration converts script (e.g., Hindi -> Latin) without translating meaning.

## 9. Responsible AI mapping

- "no bias across user groups" -> **Fairness**
- "explainability, model card, decision reason" -> **Transparency**
- "PII, encryption, customer control" -> **Privacy & Security**
- "alt text, captions, screen reader support" -> **Inclusiveness**
- "fails safely, consistent at scale" -> **Reliability & Safety**
- "human governance, audit trail, ownership" -> **Accountability**

## 10. Azure ML basic vocabulary

- **Compute instance** != **Compute cluster**. Instance = single dev VM. Cluster = autoscaling training pool.
- **Datastore** = pointer. **Dataset / Data asset** = versioned reference inside the datastore.
- **Pipeline** in Azure ML is the *training/deployment graph*, not a CI/CD pipeline (different concept than Azure DevOps Pipelines).

## 11. Question-reading habits

- Watch for **"prebuilt"** in the question -> biases toward Image Analysis / Document Intelligence prebuilt models.
- Watch for **"my own labels / company-specific"** -> biases toward Custom Vision, Custom NER, Custom Translator, Custom QnA.
- Watch for **"limited access"** or **"approved use case"** -> biases toward Face Identification, Custom Neural Voice.
- Watch for **"low code"** or **"no code"** -> biases toward AutoML, Designer, Copilot Studio.
- Watch for **"chat over our docs"** -> RAG with Foundry + Azure AI Search + OpenAI.

---

[<- Flashcards](13-flashcards.md) - [Hands-on Labs ->](15-hands-on-labs.md)
