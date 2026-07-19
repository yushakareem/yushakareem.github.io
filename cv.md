---
layout: default
title: CV
permalink: /cv/
---

<div class="cv">

<h1>yusha kareem</h1>
<p class="cv-subtitle">Senior Data Scientist | AI Engineer</p>
<p class="cv-meta">Amsterdam, Netherlands</p>

<h2>relevant expertise</h2>

<ul>
  <li><strong>Machine Learning &amp; MLOps:</strong> systems design across diverse projects; ML/GenAI delivered end-to-end with data versioning and quality checks (Great Expectations), feature engineering, training, registry and deployment (MLFlow on Databricks), and metric selection for iterative evaluation.</li>
  <li><strong>Cross-functional delivery:</strong> collaborated with data engineers, data scientists and business stakeholders to ship impactful ML solutions; coached juniors while holding a senior role.</li>
  <li><strong>Stakeholder management &amp; consulting:</strong> translate business challenges into concrete goals; manage the quick-PoC-vs-scalable-solution tradeoff; communicate clearly to technical and non-technical audiences.</li>
</ul>

<h2>skills</h2>
<p class="cv-tags">Python · Databricks · CI/CD (DevOps) · Pandas · MLFlow · Streamlit · Terraform · uv · SQL · LangGraph · RAG · Docker · Git · Docling · Azure (DevOps/ML) · GCP · Vertex AI · Scrum/Agile · scikit-learn · Great Expectations · Double Diamond · Three-lens business strategy</p>

<h2>languages</h2>
<p class="cv-tags">English (native) · Urdu (native) · Italian (beginner) · Arabic (beginner) · Dutch (beginner) · French (beginner)</p>

<h2>strengths</h2>
<p class="cv-tags">Takes ownership of initiatives · Data science, MLOps, GenAI &amp; applied research · Feedback &amp; growth mindset · Delivers technical insight to non-technical stakeholders · Published researcher (4 articles in AI &amp; robotics)</p>

<h2>experience</h2>

<div class="cv-job">
  <div class="cv-job-head">
    <span class="cv-role">AI Engineer — Deloitte <span class="cv-client">· Deloitte's SAP practice</span></span>
    <span class="cv-when">Amsterdam · 06/2026 – Present</span>
  </div>
  <p class="cv-stack">Python, FastAPI, React, GCP (Cloud Run, Vertex AI, Firestore), Gemini, Docling, RAG, Terraform, GitHub Actions, Docker</p>
  <ul>
    <li>Built a GenAI tool for Deloitte's SAP teams to expedite S/4HANA projects: auto-maps client documents to Deloitte's Ascend methodology, generates process analysis and workshop plans, and drafts grounded, client-ready deliverables.</li>
    <li>Ran use-case discovery with SAP consultants; scoped and prioritised features into a clear solution brief.</li>
    <li>Designed and built an end-to-end <strong>RAG pipeline</strong> (parse → chunk → embed → hybrid semantic + keyword search) over a file-based knowledge base.</li>
    <li><strong>Grounded generation:</strong> every claim tied to a source chunk, unsupported points surfaced as gaps (anti-hallucination); a deterministic renderer applies the client template as a soft brand reference; an automated pass verifies grounding and section coverage.</li>
    <li><strong>Parsing tradeoff:</strong> replaced page-by-page vision parsing with layout-aware parsing (Docling), sending only detected diagrams to the vision model — <strong>~40% fewer vision-model calls, ~4× faster processing</strong>, verified against real client documents.</li>
    <li><strong>Reliability &amp; cost engineering:</strong> per-task model choices (analysis vs. embeddings vs. diagrams) to balance quality, latency and cost.</li>
    <li><strong>Deployment:</strong> serverless GCP (Cloud Run scale-to-zero), IaC (Terraform), CI/CD (GitHub Actions).</li>
  </ul>
</div>

<div class="cv-job">
  <div class="cv-job-head">
    <span class="cv-role">Senior Data Scientist — Deloitte <span class="cv-client">· a global logistics company</span></span>
    <span class="cv-when">Amsterdam · 09/2025 – 03/2026</span>
  </div>
  <p class="cv-stack">Python, Databricks, XGBoost, AutoARIMA, SHAP</p>
  <ul>
    <li>Built a long-term shipping-volume <strong>forecasting system</strong> with model explainability.</li>
    <li><strong>Architecture:</strong> two-tier stacked ensemble — specialised models (e.g. AutoARIMA) blending historical volume with external factors (crude-oil prices, freight spot rates), then an XGBoost meta-learner.</li>
    <li><strong>Explainability:</strong> SHAP to rank feature importance and show how each expert model drives predictions.</li>
    <li>Improved accuracy at customer-tradelane (country-to-country) granularity across a 12-month horizon; automated the Databricks pipeline as a scheduled monthly job with frozen-forecast accuracy monitoring.</li>
  </ul>
</div>

<div class="cv-job">
  <div class="cv-job-head">
    <span class="cv-role">Senior Data Scientist — Deloitte <span class="cv-client">· a global home-furnishings retailer</span></span>
    <span class="cv-when">Amsterdam · 06/2025 – 08/2025</span>
  </div>
  <p class="cv-stack">Python, Unstructured.io, Vector DB, RAG, Hybrid Search</p>
  <ul>
    <li>Implemented an <strong>intelligent document-retrieval (RAG) system</strong> for the client's insights team, cutting manual search time and enabling cost-efficient GenAI integration.</li>
    <li>Automated ingestion of heterogeneous sources (Excel, PDF, Word, PowerPoint) incl. nested-zip extraction, dedup and preprocessing; vectorised and indexed into a vector DB; matched business questions to relevant files via hybrid scoring.</li>
  </ul>
</div>

<div class="cv-job">
  <div class="cv-job-head">
    <span class="cv-role">Senior Data Scientist — Deloitte <span class="cv-client">· two UK retailers</span></span>
    <span class="cv-when">Amsterdam · 04/2026 – 05/2026</span>
  </div>
  <p class="cv-stack">Python, Polars, statsmodels, Great Expectations, Playwright</p>
  <ul>
    <li>Delivered <strong>SKU-rationalisation analytics</strong> over large-scale weekly sales data and thousands of SKU×channel pairs to support range-review decisions.</li>
    <li>Built a config-driven <strong>category-management dashboard</strong>: competitor hierarchy and prices via web scraping (Playwright); range optimisation (Pareto — the ~20% of SKUs driving ~80% of revenue) and price optimisation (elasticity + promo scenarios), with price/volume forecasting scaffolded next.</li>
  </ul>
</div>

<div class="cv-job">
  <div class="cv-job-head">
    <span class="cv-role">Senior Data Scientist — Deloitte <span class="cv-client">· PriceCypher (client: a Dutch food &amp; bio-chemicals producer)</span></span>
    <span class="cv-when">Amsterdam · 11/2023 – 03/2025</span>
  </div>
  <p class="cv-stack">Python, PYGAM, MLFlow, Argo Workflows, Great Expectations, Azure DevOps/Pipelines, uv</p>
  <ul>
    <li>Led the end-to-end revamp of <strong>PriceCypher's</strong> ML-based pricing model, increasing potential revenue for the client.</li>
    <li><strong>Modelling:</strong> price–volume relationship per product via a constrained Generalised Additive Model (GAM) for interpretability.</li>
    <li><strong>MLOps:</strong> data-quality checks (Great Expectations); MLFlow for packaging, versioning and serving.</li>
  </ul>
</div>

<div class="cv-job">
  <div class="cv-job-head">
    <span class="cv-role">Data Scientist — Deloitte <span class="cv-client">· an engineering &amp; steel-production company</span></span>
    <span class="cv-when">Amsterdam · 09/2022 – 12/2022</span>
  </div>
  <p class="cv-stack">Python, Databricks, MLFlow, LightGBM, Azure Pipelines</p>
  <ul>
    <li>Built a <strong>demand-forecasting tool for car parts</strong> to optimise production scheduling and inventory; selected LightGBM after it outperformed alternatives; MVP adopted by the client for real-world testing.</li>
  </ul>
</div>

<div class="cv-job">
  <div class="cv-job-head">
    <span class="cv-role">Data Scientist — Deloitte <span class="cv-client">· The Ocean Cleanup (environmental NGO)</span></span>
    <span class="cv-when">Rotterdam · 02/2022 – 08/2022</span>
  </div>
  <p class="cv-stack">Python, YOLOv5, AzureML</p>
  <ul>
    <li>Enhanced The Ocean Cleanup's <strong>computer-vision model</strong> detecting plastic on river surfaces — improved mAP <strong>67% → 87%</strong> via targeted data augmentation and retraining.</li>
    <li>Built an <strong>object-tracking module</strong> estimating monthly river-to-ocean plastic volume, helping allocate interceptor boats and plan operations.</li>
  </ul>
</div>

<h2>mentoring</h2>

<div class="cv-job">
  <div class="cv-job-head">
    <span class="cv-role">Data-science mentor — Deloitte Impact Foundation / SpikeUp AI</span>
    <span class="cv-when">Amsterdam · 03/2023 – 12/2025</span>
  </div>
  <ul>
    <li>Help highly educated refugees build careers in data science; mentored three through training into professional roles.</li>
  </ul>
</div>

<h2>education</h2>

<div class="cv-job">
  <div class="cv-job-head">
    <span class="cv-role">PhD, Robotics &amp; Autonomous Systems <span class="cv-client">· University of Genova, Italy</span></span>
    <span class="cv-when">2017 – 2021</span>
  </div>
  <ul>
    <li>AI framework for human-activity recognition in a smart home, combining knowledge-graph reasoning with ML inference for explainable AI. 4 peer-reviewed publications. Taught ROS as a teaching assistant.</li>
  </ul>
</div>

<div class="cv-job">
  <div class="cv-job-head">
    <span class="cv-role">MSc, Robotics Engineering <span class="cv-client">· École Centrale de Nantes &amp; University of Genova</span></span>
    <span class="cv-when">2015 – 2017</span>
  </div>
  <ul>
    <li>Erasmus dual-degree EMARO+ (European Master on Advanced Robotics).</li>
  </ul>
</div>

<div class="cv-job">
  <div class="cv-job-head">
    <span class="cv-role">BEng, Mechanical Engineering <span class="cv-client">· M.S.R. Institute of Technology, Bangalore, India</span></span>
    <span class="cv-when">2010 – 2014</span>
  </div>
  <ul>
    <li>Led the university team to 1st place (all universities, southern India) in the Autodesk Inventor design competition.</li>
  </ul>
</div>

</div>
