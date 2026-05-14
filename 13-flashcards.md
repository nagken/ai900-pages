# Flashcards: Active Recall

> Click any card to reveal the answer. Use the **Domain pager bottom-right** to switch between exam areas.

<section class="fc-section" data-fc-title="AI Workloads + Responsible AI">
<h2>1 - AI Workloads + Responsible AI</h2>

<div class="flashcard-grid">

<div class="flashcard"><div class="fc-q">Name the six Microsoft Responsible AI principles.</div><div class="fc-a"><strong>Fairness, Reliability &amp; Safety, Privacy &amp; Security, Inclusiveness, Transparency, Accountability.</strong></div></div>

<div class="flashcard"><div class="fc-q">Which principle covers explainability and model cards?</div><div class="fc-a"><strong>Transparency.</strong></div></div>

<div class="flashcard"><div class="fc-q">Which principle covers protecting user data and access controls?</div><div class="fc-a"><strong>Privacy &amp; Security.</strong></div></div>

<div class="flashcard"><div class="fc-q">Which principle requires the model to work the same across genders, races, regions?</div><div class="fc-a"><strong>Fairness.</strong></div></div>

<div class="flashcard"><div class="fc-q">Which principle is invoked when an AI system needs alt text and captions for accessibility?</div><div class="fc-a"><strong>Inclusiveness.</strong></div></div>

<div class="flashcard"><div class="fc-q">Name the five AI workload categories on AI-900.</div><div class="fc-a">Computer Vision, NLP, Document Intelligence / Knowledge Mining, Generative AI, Machine Learning. (Anomaly detection sometimes listed separately.)</div></div>

</div>
</section>

<section class="fc-section" data-fc-title="Machine Learning">
<h2>2 - Machine Learning</h2>

<div class="flashcard-grid">

<div class="flashcard"><div class="fc-q">Predict house price - what ML problem type?</div><div class="fc-a"><strong>Regression</strong> (numeric prediction).</div></div>

<div class="flashcard"><div class="fc-q">Predict spam vs not spam - what ML problem type?</div><div class="fc-a"><strong>Classification</strong> (binary).</div></div>

<div class="flashcard"><div class="fc-q">Group customers without predefined labels - what type?</div><div class="fc-a"><strong>Clustering</strong> (unsupervised).</div></div>

<div class="flashcard"><div class="fc-q">Detect rare fraudulent transactions - what type?</div><div class="fc-a"><strong>Anomaly detection</strong>.</div></div>

<div class="flashcard"><div class="fc-q">What's the difference between feature and label?</div><div class="fc-a"><strong>Feature</strong> = input column. <strong>Label</strong> = target the model predicts.</div></div>

<div class="flashcard"><div class="fc-q">When is accuracy a misleading classification metric?</div><div class="fc-a">On <strong>imbalanced data</strong>. Use precision / recall / F1 / AUC instead.</div></div>

<div class="flashcard"><div class="fc-q">What does Automated ML automate?</div><div class="fc-a">Iterates over <strong>algorithm + hyperparameter + featurization</strong> to find the best model for your dataset and primary metric.</div></div>

<div class="flashcard"><div class="fc-q">Difference between real-time and batch endpoint?</div><div class="fc-a"><strong>Real-time</strong> = single requests, low latency. <strong>Batch</strong> = score large dataset asynchronously.</div></div>

<div class="flashcard"><div class="fc-q">Three regression metrics?</div><div class="fc-a"><strong>MAE</strong>, <strong>RMSE</strong>, <strong>R^2</strong>.</div></div>

</div>
</section>

<section class="fc-section" data-fc-title="Computer Vision">
<h2>3 - Computer Vision</h2>

<div class="flashcard-grid">

<div class="flashcard"><div class="fc-q">Tag images with prebuilt categories - which service?</div><div class="fc-a"><strong>Azure AI Vision - Image Analysis 4.0</strong>.</div></div>

<div class="flashcard"><div class="fc-q">Train an image classifier on your own labels - which service?</div><div class="fc-a"><strong>Custom Vision</strong>.</div></div>

<div class="flashcard"><div class="fc-q">Read printed + handwritten text - which feature?</div><div class="fc-a"><strong>Azure AI Vision - Read API (OCR)</strong>.</div></div>

<div class="flashcard"><div class="fc-q">Identify a specific person from a photo - which service + access tier?</div><div class="fc-a"><strong>Azure AI Face - Identification</strong>. <strong>Limited Access</strong> (must apply for approval).</div></div>

<div class="flashcard"><div class="fc-q">Extract vendor + total + line items from an invoice - which service?</div><div class="fc-a"><strong>Azure AI Document Intelligence - prebuilt invoice model</strong>.</div></div>

<div class="flashcard"><div class="fc-q">Auto-generate captions and chapters for a meeting recording - which service?</div><div class="fc-a"><strong>Azure Video Indexer</strong>.</div></div>

<div class="flashcard"><div class="fc-q">Were emotion / age / gender attributes in Face retired?</div><div class="fc-a"><strong>Yes</strong>, retired in 2022. Don't pick them on the exam.</div></div>

<div class="flashcard"><div class="fc-q">What was Azure AI Document Intelligence formerly called?</div><div class="fc-a"><strong>Form Recognizer</strong>.</div></div>

</div>
</section>

<section class="fc-section" data-fc-title="Natural Language Processing">
<h2>4 - Natural Language Processing</h2>

<div class="flashcard-grid">

<div class="flashcard"><div class="fc-q">Detect language of incoming text - which feature?</div><div class="fc-a"><strong>Azure AI Language - Language detection</strong>.</div></div>

<div class="flashcard"><div class="fc-q">Extract People / Org / Location entities - which feature?</div><div class="fc-a"><strong>Named Entity Recognition (NER)</strong>.</div></div>

<div class="flashcard"><div class="fc-q">Build a chatbot that recognizes intents and slots - which feature?</div><div class="fc-a"><strong>Conversational Language Understanding (CLU)</strong> - replaces LUIS.</div></div>

<div class="flashcard"><div class="fc-q">Build an FAQ bot from PDF docs - which feature?</div><div class="fc-a"><strong>Custom Question Answering</strong> - replaces QnA Maker.</div></div>

<div class="flashcard"><div class="fc-q">Translate a Word doc keeping all formatting - which feature?</div><div class="fc-a"><strong>Document Translation</strong> in Azure AI Translator.</div></div>

<div class="flashcard"><div class="fc-q">Translate spoken English audio to spoken Spanish audio - which service?</div><div class="fc-a"><strong>Azure AI Speech - Speech Translation</strong>. (Not Translator.)</div></div>

<div class="flashcard"><div class="fc-q">Brand-specific TTS voice for IVR - which feature + access?</div><div class="fc-a"><strong>Custom Neural Voice</strong>. <strong>Limited Access</strong>.</div></div>

<div class="flashcard"><div class="fc-q">Aspect-level sentiment ("food positive, service negative") - which feature?</div><div class="fc-a"><strong>Opinion mining</strong> in sentiment analysis.</div></div>

<div class="flashcard"><div class="fc-q">Real-time captions in a Teams call - which feature?</div><div class="fc-a"><strong>Speech to Text (real-time)</strong>.</div></div>

</div>
</section>

<section class="fc-section" data-fc-title="Generative AI">
<h2>5 - Generative AI</h2>

<div class="flashcard-grid">

<div class="flashcard"><div class="fc-q">What replaced Azure AI Studio?</div><div class="fc-a"><strong>Azure AI Foundry</strong>.</div></div>

<div class="flashcard"><div class="fc-q">What is a token?</div><div class="fc-a">Chunk of text the model processes (~3/4 of an English word). Pricing unit.</div></div>

<div class="flashcard"><div class="fc-q">What's an embedding?</div><div class="fc-a">A <strong>vector</strong> representing the meaning of text or an image. Used for similarity search and RAG.</div></div>

<div class="flashcard"><div class="fc-q">When do you use RAG vs fine-tuning?</div><div class="fc-a"><strong>RAG</strong> for ground-on-our-docs / latest data / cite sources. <strong>Fine-tune</strong> to change style or behavior.</div></div>

<div class="flashcard"><div class="fc-q">What does Prompt Shields protect against?</div><div class="fc-a"><strong>Jailbreak</strong> (user injection) and <strong>document attacks</strong> (poisoned RAG chunks).</div></div>

<div class="flashcard"><div class="fc-q">Which Azure feature flags hallucinations against source data?</div><div class="fc-a"><strong>Groundedness detection</strong> in Azure AI Content Safety.</div></div>

<div class="flashcard"><div class="fc-q">What service do you pick for a low-code custom HR copilot?</div><div class="fc-a"><strong>Microsoft Copilot Studio</strong>.</div></div>

<div class="flashcard"><div class="fc-q">Where do you call OpenAI models in Azure?</div><div class="fc-a">Through <strong>Azure OpenAI Service</strong>, accessed via Azure AI Foundry projects.</div></div>

<div class="flashcard"><div class="fc-q">Name the four Content Safety harm categories.</div><div class="fc-a"><strong>Hate</strong>, <strong>Sexual</strong>, <strong>Violence</strong>, <strong>Self-harm</strong>.</div></div>

</div>
</section>

---

[<- Glossary](12-glossary.md) - [Pitfalls ->](14-pitfalls.md)
