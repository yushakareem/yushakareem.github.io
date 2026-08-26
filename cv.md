---
layout: default
title: CV
permalink: /cv/
---

<div class="cv">

<h1>yusha kareem</h1>
<p class="cv-subtitle">Senior AI Engineer</p>
<p class="cv-meta">Amsterdam, Netherlands</p>

<h2 id="expertise">expertise</h2>

<ul>
  <li><strong>GenAI, Machine Learning and MLOps:</strong> overall systems thinking experience across diverse projects, taking ownership of diverse aspects of the end-to-end delivery — architecture design, core modelling (selection of metrics, training, evaluation and inference), data preparation and quality checks, and dashboarding.</li>
  <li><strong>Cross-functional delivery:</strong> collaboration with business stakeholders, business analysts and data engineers to ship AI solutions; coached juniors when having a senior role on a project.</li>
  <li><strong>Stakeholder management &amp; consulting:</strong> use-case discovery, scoping and translation of business requirements into concrete development goals; communicating clearly with technical and non-technical audiences; presenting work at learn and share events.</li>
</ul>

<h2 id="skills">skills</h2>
<p class="cv-tags">Python · Databricks · CI/CD (DevOps) · Pandas · MLFlow · Streamlit · Terraform · uv · SQL · LangGraph · RAG · Docker · Git · Docling · Azure (DevOps/ML) · GCP · Vertex AI · Scrum/Agile · scikit-learn · Great Expectations · Double Diamond · Three-lens business strategy</p>

<h2 id="languages">languages</h2>
<p class="cv-tags">English (native) · Urdu (native) · Italian (beginner) · Arabic (beginner) · Dutch (beginner) · French (beginner)</p>

<h2 id="strengths">strengths</h2>
<p class="cv-tags">Takes ownership of initiatives · Data science, MLOps, GenAI &amp; applied research · Feedback &amp; growth mindset · Delivers technical insight to non-technical stakeholders · Published researcher (4 articles in AI &amp; robotics)</p>

<h2 id="experience">relevant experience</h2>

<div class="cv-job">
  <aside class="note"><span class="note-when">Amsterdam · 05/2026 – present</span><span class="note-stack">Python · FastAPI · React · GCP (Cloud Run, Vertex AI, Firestore, Cloud Storage) · Gemini (3.1 Pro, embedding-001) · Docling · python-pptx/python-docx/openpyxl · RAG · Terraform · GitHub Actions · Docker</span></aside>
  <div class="cv-job-head">
    <span class="cv-role">AI Engineer — Deloitte <span class="cv-client">· Deloitte's SAP practice</span></span>
  </div>
  <ul>
    <li>Built a GenAI tool that saves Deloitte's SAP consultants hours of manual work on every S/4HANA implementation project — instead of sifting through meeting notes, client documentation and SAP standard practice by hand, they get an automatic view of what the client's documents do and don't cover, plus first drafts of the deliverables (Word, PowerPoint, Excel) across each phase.</li>
    <li><strong>Use-case discovery:</strong> ran discovery sessions with SAP consultants to map their process and pain points, qualified what was feasible and high-value, and scoped/prioritised features into a clear solution brief.</li>
    <li><strong>Retrieval (RAG):</strong> built the pipeline that makes this possible — client documents are parsed, split into passages and indexed, and the most relevant ones are retrieved per request using a combination of meaning-based and keyword search, so the tool writes only from the client's own material.</li>
    <li><strong>Grounded draft deliverables:</strong> designed a two-step approach where the model first produces a plan in which every point must cite the passage it came from; anything it cannot support surfaces as a visible gap for the consultant to fill, rather than being invented. Each deliverable stores its plan and sources so any output can be traced back later.</li>
    <li><strong>Cloud deployment:</strong> serverless on GCP (Cloud Run, scale-to-zero) with infrastructure-as-code (Terraform), automated CI/CD (GitHub Actions), and a storage layer that runs identically locally and in the cloud.</li>
    <li><strong>Safe automation:</strong> the code that assembles each document is model-generated but never trusted — it runs inside a locked-down sandbox with no file or network access, a hard time limit, and automatic retry on failure.</li>
    <li><strong>Quality, cost &amp; latency:</strong> tuned prompts per task to keep output consistent across a large set of analyses, and matched each task to the right model, balancing quality against speed and cost.</li>
  </ul>
</div>

<div class="cv-job">
  <aside class="note"><span class="note-when">Amsterdam · 09/2025 – 03/2026</span><span class="note-stack">Python · Databricks (Jobs, MLFlow, SQL) · XGBoost · AutoARIMA · Prophet · SHAP · Pandas · NumPy</span></aside>
  <div class="cv-job-head">
    <span class="cv-role">Senior Data Scientist — Deloitte <span class="cv-client">· a global logistics company</span></span>
  </div>
  <ul>
    <li>Built a long-term shipping-volume <strong>forecasting system</strong>, with model explainability.</li>
    <li><strong>Architecture redesign:</strong> moved from a single-model approach to a two-tier stacked ensemble — specialised models (AutoARIMA, Prophet) combining historical volume with external factors (crude-oil prices, freight spot rates), then an XGBoost meta-learner to combine their predictions.</li>
    <li><strong>Explainability:</strong> integrated SHAP to rank feature importance and show how much each expert model (e.g. crude-oil vs. spot-rate agent) drives the prediction.</li>
    <li><strong>Impact:</strong> improved accuracy at customer-tradelane (country-to-country) granularity across a 12-month horizon; multiple departments now rely on the long-term forecast.</li>
    <li><strong>Pipeline automation:</strong> automated the end-to-end pipeline in Databricks (SQL ingestion, training, prediction, SHAP) as a scheduled monthly job.</li>
    <li><strong>Accuracy monitoring:</strong> applied a frozen-forecast evaluation — locking each month's forecast at generation time and comparing it against the actual volume that eventually shipped.</li>
  </ul>
</div>

<div class="cv-job">
  <aside class="note"><span class="note-when">Amsterdam · 06/2025 – 08/2025</span><span class="note-stack">Python · Unstructured.io · Vector DB · RAG · Hybrid Search</span></aside>
  <div class="cv-job-head">
    <span class="cv-role">Senior Data Scientist — Deloitte <span class="cv-client">· a global home-furnishings retailer</span></span>
  </div>
  <ul>
    <li>Implemented an <strong>intelligent document-retrieval (RAG) system</strong> for the client's insights team, cutting manual search time and enabling cost-efficient GenAI integration.</li>
    <li><strong>Architecture &amp; scoping:</strong> designed the architecture — functional vs. non-functional requirements, prioritising features into must-have, nice-to-have and future-work.</li>
    <li><strong>Ingestion:</strong> automated ingestion of heterogeneous sources (Excel, PDF, Word, PowerPoint), including nested-zip extraction, deduplication and preprocessing via unstructured.io.</li>
    <li><strong>Semantic search:</strong> vectorised and indexed documents into a vector DB for efficient semantic search.</li>
    <li><strong>Data-gap assessment:</strong> matched business questions to relevant files via hybrid scoring, returning focused sets of high-confidence documents for RAG.</li>
  </ul>
</div>

<div class="cv-job">
  <aside class="note"><span class="note-when">Amsterdam · 04/2026 – 05/2026</span><span class="note-stack">Python · Polars · Pandas · statsmodels · Great Expectations · Playwright · Parquet</span></aside>
  <div class="cv-job-head">
    <span class="cv-role">Senior Data Scientist — Deloitte <span class="cv-client">· two UK retailers</span></span>
  </div>
  <ul>
    <li>Delivered <strong>SKU-rationalisation analytics</strong> for two UK retailers — ~12M rows of weekly sales data for one, ~9,000 SKU×channel pairs for the other — to support range-review decisions.</li>
    <li>Built a config-driven <strong>category-management control centre</strong> consolidating the range-review workflow into one dashboard: competitor category hierarchy, product details and prices collected via web scraping (Playwright); range optimisation (Pareto analysis — the ~20% of SKUs driving ~80% of revenue) and price optimisation (elasticity + promo scenarios), with price/volume forecasting from long-term data scaffolded as the next module.</li>
  </ul>
</div>

<div class="cv-job">
  <aside class="note"><span class="note-when">Amsterdam · 11/2023 – 03/2025</span><span class="note-stack">Python · Pandas · NumPy · PYGAM · MLFlow · Argo Workflows · Great Expectations · Azure DevOps/Pipelines · uv</span></aside>
  <div class="cv-job-head">
    <span class="cv-role">Senior Data Scientist — Deloitte <span class="cv-client">· PriceCypher (client: a Dutch food &amp; bio-chemicals producer)</span></span>
  </div>
  <ul>
    <li>Led the end-to-end revamp of <strong>PriceCypher's</strong> ML-based pricing model, resulting in €12M in potential revenue for the client.</li>
    <li><strong>Modelling:</strong> price–volume relationship per product via a constrained Generalised Additive Model (GAM) for interpretability.</li>
    <li><strong>MLOps:</strong> data-quality checks (Great Expectations); MLFlow for packaging, versioning and serving.</li>
  </ul>
</div>

<div class="cv-job">
  <aside class="note"><span class="note-when">Amsterdam · 09/2022 – 12/2022</span><span class="note-stack">Python · Databricks · MLFlow · LightGBM · Azure Pipelines</span></aside>
  <div class="cv-job-head">
    <span class="cv-role">Data Scientist — Deloitte <span class="cv-client">· an engineering &amp; steel-production company</span></span>
  </div>
  <ul>
    <li>Built a <strong>demand-forecasting tool for car parts</strong> to optimise production scheduling and inventory; selected LightGBM after it outperformed alternatives; MVP adopted by the client for real-world testing.</li>
  </ul>
</div>

<div class="cv-job">
  <aside class="note"><span class="note-when">Rotterdam · 02/2022 – 08/2022</span><span class="note-stack">Python · YOLOv5 · AzureML · Git</span></aside>
  <div class="cv-job-head">
    <span class="cv-role">Data Scientist — Deloitte <span class="cv-client">· The Ocean Cleanup (environmental NGO)</span></span>
  </div>
  <ul>
    <li>Enhanced The Ocean Cleanup's <strong>computer-vision model</strong> detecting plastic on river surfaces — improved mAP <strong>67% → 87%</strong> via targeted data augmentation and retraining.</li>
    <li>Built an <strong>object-tracking module</strong> estimating monthly river-to-ocean plastic volume, helping allocate interceptor boats and plan operations.</li>
  </ul>
</div>

<h2 id="mentoring">mentoring</h2>

<div class="cv-job">
  <aside class="note"><span class="note-when">Amsterdam · 03/2023 – 12/2025</span></aside>
  <div class="cv-job-head">
    <span class="cv-role">Data-science mentor — Deloitte Impact Foundation / SpikeUp AI</span>
  </div>
  <ul>
    <li>Help highly educated refugees build careers in data science; mentored three through training into professional roles.</li>
  </ul>
</div>

<h2 id="education">academics</h2>

<div class="cv-job">
  <aside class="note"><span class="note-when">2017 – 2021</span></aside>
  <div class="cv-job-head">
    <span class="cv-role">PhD, Robotics &amp; Autonomous Systems <span class="cv-client">· University of Genova, Italy</span></span>
  </div>
  <ul>
    <li><strong>Research topic 'Knowledge Graph based reasoning':</strong> designed an AI framework for human-activity recognition in a smart home, combining knowledge-graph reasoning (formal logic) with machine-learning inference for explainable AI.</li>
    <li><strong>Publications:</strong> published 4 research articles in peer-reviewed journals.</li>
    <li><strong>Teaching:</strong> as a teaching assistant, taught first-year master's students to use Robot Operating System (ROS) to integrate robot perception, reasoning and action.</li>
  </ul>
</div>

<div class="cv-job">
  <aside class="note"><span class="note-when">2015 – 2017</span></aside>
  <div class="cv-job-head">
    <span class="cv-role">MSc, Robotics Engineering <span class="cv-client">· École Centrale de Nantes &amp; University of Genova</span></span>
  </div>
  <ul>
    <li>Erasmus dual-degree EMARO+ (European Master on Advanced Robotics).</li>
  </ul>
</div>

<div class="cv-job">
  <aside class="note"><span class="note-when">2010 – 2014</span></aside>
  <div class="cv-job-head">
    <span class="cv-role">BEng, Mechanical Engineering <span class="cv-client">· M.S.R. Institute of Technology, Bangalore, India</span></span>
  </div>
  <ul>
    <li>Led the university team to 1st place (all universities, southern India) in the Autodesk Inventor design competition.</li>
  </ul>
</div>

</div>
