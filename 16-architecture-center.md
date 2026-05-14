# Architecture Center - AI-900 reading list

> Curated reference architectures from [learn.microsoft.com/azure/architecture](https://learn.microsoft.com/azure/architecture). Skim each - AI-900 expects diagram-level recognition, not implementation detail.

## Generative AI

- [Baseline OpenAI end-to-end chat reference architecture](https://learn.microsoft.com/azure/architecture/ai-ml/architecture/baseline-openai-e2e-chat) - gold-standard RAG topology with App Service, Azure AI Search, Azure OpenAI, Key Vault, Private Endpoints.
- [OpenAI chat baseline architecture in an Azure landing zone](https://learn.microsoft.com/azure/architecture/ai-ml/architecture/azure-openai-baseline-landing-zone) - landing-zone variant.
- [Build a custom copilot using Azure AI Foundry](https://learn.microsoft.com/azure/architecture/ai-ml/architecture/build-chatbot-azure-openai) - Foundry-centric reference.
- [Azure OpenAI batch processing reference](https://learn.microsoft.com/azure/architecture/ai-ml/idea/azure-openai-batch) - batch vs real-time inference patterns.
- [RAG fundamentals on Azure AI Search](https://learn.microsoft.com/azure/search/retrieval-augmented-generation-overview) - index -> embed -> retrieve -> ground.

## Knowledge mining

- [Knowledge mining for content research](https://learn.microsoft.com/azure/architecture/solution-ideas/articles/knowledge-mining-content-research) - Azure AI Search + skillsets.
- [Knowledge mining in business process management](https://learn.microsoft.com/azure/architecture/solution-ideas/articles/business-process-management).

## Document and form processing

- [Automate document processing with Azure AI Document Intelligence](https://learn.microsoft.com/azure/architecture/ai-ml/architecture/automate-document-processing-azure-form-recognizer) - invoice / receipt automation pipeline.
- [Suggested content with custom NLP](https://learn.microsoft.com/azure/architecture/solution-ideas/articles/article-recommendation-with-cognitive-services).

## Conversational AI

- [Enterprise-grade conversational bot](https://learn.microsoft.com/azure/architecture/solution-ideas/articles/conversational-bot) - Bot Service + Language + LUIS/CLU + QnA/CQA.
- [Commerce chatbot for customer service](https://learn.microsoft.com/azure/architecture/solution-ideas/articles/commerce-chatbot).

## Computer vision

- [Image classification on Azure](https://learn.microsoft.com/azure/architecture/ai-ml/architecture/intelligent-apps-image-processing) - vision pipeline pattern.
- [Vehicle telemetry analytics](https://learn.microsoft.com/azure/architecture/solution-ideas/articles/vehicle-telematics-analytics-solution) - vision + IoT.

## Speech and translation

- [Customer service call transcription and analysis](https://learn.microsoft.com/azure/architecture/ai-ml/architecture/speech-to-text-transcription-pipelines) - Speech + Language pipeline.
- [Translation pipeline for global apps](https://learn.microsoft.com/azure/architecture/solution-ideas/articles/translator-text-pipeline).

## Machine learning

- [MLOps with Azure ML](https://learn.microsoft.com/azure/architecture/ai-ml/guide/mlops-technical-paper) - versioning, CI/CD, retraining.
- [Modern data warehouse for ML](https://learn.microsoft.com/azure/architecture/solution-ideas/articles/modern-data-warehouse-for-machine-learning) - ADLS + Synapse + Azure ML.
- [Real-time scoring of ML models](https://learn.microsoft.com/azure/architecture/ai-ml/architecture/real-time-scoring-machine-learning-models) - managed online endpoint.
- [Batch scoring of ML models](https://learn.microsoft.com/azure/architecture/ai-ml/architecture/batch-scoring-python).

## Cross-cutting

- [Choose an Azure AI services technology](https://learn.microsoft.com/azure/architecture/data-guide/technology-choices/cognitive-services) - decision flowchart you should be able to draw from memory.
- [Cloud Adoption Framework - AI scenarios](https://learn.microsoft.com/azure/cloud-adoption-framework/scenarios/ai/) - governance perspective.
- [Azure Well-Architected Framework - AI workloads](https://learn.microsoft.com/azure/well-architected/ai/) - five pillars applied to AI.

---

## How to read these for AI-900

1. Open each diagram. Cover the captions.
2. Name every box from memory. If you can't, pause and look it up.
3. Trace data flow with your finger; describe each arrow out loud.
4. Note auth and storage choices (Key Vault, Managed Identity, Private Endpoint, Blob, AI Search).
5. Move to the next.

---

[<- Hands-on Labs](15-hands-on-labs.md) - [AI Copilot Quiz ->](17-copilot-quiz.md)
