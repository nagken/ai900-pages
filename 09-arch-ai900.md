# AI-900 Reference Architectures

> Concept-level architecture diagrams for the patterns AI-900 expects you to recognize. Each diagram is paired with a "what's happening" caption and "when to pick it" cues.

## 1. Prebuilt AI services - single API call

```mermaid
flowchart LR
    User[User / App] --> Front[Frontend or API]
    Front --> Key[API key or Entra token]
    Key --> AI[Azure AI service<br/>Vision / Language / Speech / Translator]
    AI --> Resp[Response: tags / sentiment / transcript / translation]
```

> Pick when an out-of-the-box capability covers the task. No training, no infra.

## 2. Custom Vision (or Custom NER / Custom Translator) - bring your own data

```mermaid
flowchart LR
    Data[Labeled samples] --> Train[Train iteration in portal / SDK]
    Train --> Eval[Evaluate metrics]
    Eval --> Pub[Publish iteration as endpoint]
    App[App] --> Pub
    Pub --> Out[Predictions on new data]
```

> Pick when prebuilt categories don't fit (your defect classes, your form types, your domain vocabulary).

## 3. Custom Question Answering - FAQ bot

```mermaid
flowchart LR
    Source[FAQ docs<br/>Web pages, PDF, DOCX] --> KB[Custom Question Answering<br/>knowledge base]
    KB --> Test[Test pane]
    Test --> Pub[Publish to prediction endpoint]
    Bot[Bot Service / web app] --> Pub
    User[User] --> Bot
    Pub --> Bot
```

> Pick for "answer questions from a fixed set of policy documents".

## 4. Conversational Language Understanding (CLU) - intent bot

```mermaid
flowchart LR
    Utter["User utterance:<br/>'Book a flight from Seattle to NYC tomorrow'"] --> CLU[Azure AI Language<br/>CLU project]
    CLU --> Intent[Intent: BookFlight]
    CLU --> Entities[Entities: origin=Seattle,<br/>destination=NYC,<br/>date=tomorrow]
    Intent --> Bot[Bot logic]
    Entities --> Bot
    Bot --> Action[Call backend / API]
```

> Pick when the bot needs to recognize *what the user wants to do* and extract structured slots.

## 5. End-to-end Azure ML - train, register, deploy

```mermaid
flowchart LR
    DS[Datastore + Dataset] --> Compute[Compute cluster]
    Compute --> Train[Training job]
    Train --> Reg[Registered model]
    Reg --> RT[Real-time endpoint<br/>online deployment]
    Reg --> BT[Batch endpoint]
    Pipe[ML pipeline orchestrates steps] -.-> Train
    Mon[Drift monitoring] -.-> RT
```

> Pick for a custom ML model lifecycle.

## 6. RAG - Retrieval Augmented Generation (the canonical Gen AI architecture)

```mermaid
flowchart LR
    Docs[Your docs:<br/>SharePoint, Blob, SQL] --> Chunk[Chunk + embed]
    Chunk --> Idx[Azure AI Search<br/>vector + keyword index]

    User[User] --> App[Web / Teams app]
    App --> Embed[Embed query<br/>text-embedding-3]
    Embed --> Search[Search Idx]
    Search --> Top[Top-k chunks]
    Top --> Prompt[Prompt builder<br/>system + question + chunks]
    Prompt --> LLM[Azure OpenAI<br/>GPT-4o]
    LLM --> Answer[Grounded answer<br/>+ citations]
    Answer --> App

    Idx -.-> Search
```

> Pick for "chat over our docs" / "make sure the bot only uses our knowledge".

## 7. Generative AI app - full responsible-AI stack

```mermaid
flowchart LR
    User[User] --> AppIn[App input]
    AppIn --> PS[Prompt Shields]
    PS --> RAG[RAG retrieval]
    RAG --> LLM[Azure OpenAI / Foundry]
    LLM --> CSO[Content Safety on output]
    CSO --> GR[Groundedness detection]
    GR --> AppOut[Response]

    Logs[App Insights / Foundry tracing] -.-> PS
    Logs -.-> CSO
    Logs -.-> GR
```

> Pick when the question mentions multiple safety layers, audit, or governance.

## 8. Knowledge Mining - Azure AI Search with built-in skills

```mermaid
flowchart LR
    Blob[Blob: PDFs, scans, audio] --> Ingest[Indexer]
    Ingest --> SS[Skillset:<br/>OCR, key phrases,<br/>language detect, custom skill]
    SS --> Idx[Search index]
    Idx --> UI[Search UI / Power BI]
```

> Pick for "search across millions of unstructured documents". Pre-Gen-AI but still valid.

## 9. Document Intelligence - invoice processing

```mermaid
flowchart LR
    Email[Inbox / SFTP / Blob] --> Trig[Logic App / Function trigger]
    Trig --> DI[Document Intelligence<br/>prebuilt-invoice]
    DI --> Fields[Extract vendor, total,<br/>line items]
    Fields --> ERP[ERP / database]
    Fields --> HIL[Human review<br/>if confidence < threshold]
    HIL --> ERP
```

> Pick for "automate invoice / receipt / ID processing".

## 10. Speech-driven contact center analytics

```mermaid
flowchart LR
    Calls[Call recordings] --> Speech[Speech to Text<br/>batch transcription]
    Speech --> Lang[Azure AI Language]
    Lang --> Senti[Sentiment]
    Lang --> Sum[Conversational summarization]
    Lang --> PII[PII redaction]
    Lang --> Topics[Key phrases / topics]
    Senti --> BI[Power BI / dashboards]
    Sum --> CRM[Update CRM]
    PII --> Lake[Compliant data lake]
```

> Pick when a question chains multiple Azure AI services to analyze calls.

---

[<- Learn Summaries](08-learn-summaries.md) - [Microsoft Resources ->](11-microsoft-resources.md)
