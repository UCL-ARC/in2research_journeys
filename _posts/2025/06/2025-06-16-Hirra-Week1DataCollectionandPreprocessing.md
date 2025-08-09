---
title: Week 1 – Data Collection and Pre-processing
date: 2025-06-16
time: "11:30"
author: hirraa
categories: ["NLP", "Preprocessing", "COVID-19", "Pharmacovigilance"]
layout: post
---

### What my project is about:

My project uses Natural language processing (NLP) to detect sentiment and feedback in social media data. During the first week, I focused on reading academic papers and exploring different topics to understand the landscape of NLP applications in health. I’m particularly interested in health related discussions on social media, where people often share personal experiences, concerns and opinions that can be valuable for research and public health monitoring. 

**The two topics I want to explore are**:

**Adverse drug reactions (ADRs**) 💊🫨 – ADRs are harmful or unwanted effects of medications. Monitoring them is an essential part of pharmacovigilance, which aims to ensure drug safety after a product is released. Pharmaceutical companies carry out post market surveillance to detect ADRs, but social media offers a real time source of additional signals that could complement traditional clinical reporting systems.

**Sentiment towards COVID-19** 🦠📱 – Analysing how people feel and what they say about COVID-19 can provide insights into public perception, compliance with health measures and the spread of misinformation. There are many labelled COVID-19 datasets available, which makes it possible to experiment with different NLP techniques for sentiment analysis at scale.

**ADRs remain an important public health issue, and with the availability of COVID-19 data, these two areas together represent a valuable and relevant direction for research** 🌐📱

---

### Datasets:

I found several datasets, some already labelled and others self-labelled, that I will use for my project.

**ADR Datasets:**

⭐ [**CADEC v2**](https://data.csiro.au/collection/csiro:62387) – Annotated patient forum posts covering drug mentions, adverse drug reactions (ADRs), symptoms and diseases.  
⭐ [**PsyTAR**](https://www.sciencedirect.com/science/article/pii/S2352340919301891) – Patient drug reviews for psychiatric medications, labelled for ADRs, withdrawal symptoms, drug effectiveness and indications.  
⭐ **Reddit health and medication subreddits** – Self-scraped and manually labelled posts for ADR mentions.  

**COVID-19 Datasets:**

⭐ [**COVID-19 Vaccine Tweets**](https://www.kaggle.com/datasets/datasciencetool/covid19-vaccine-tweets-with-sentiment-annotation/data) – Tweets related to COVID-19 vaccines with sentiment annotations.  
⭐ **Reddit COVID-19 subreddits** – Scraped posts, labelled for COVID-19 sentiment.  
⭐ [**Instagram COVID-19 Posts**](https://www.kaggle.com/datasets/thakurnirmalya/covid-19-sentiment-500k-instagram-posts-2020-24) –  posts tagged with COVID-19, labelled for sentiment.

---

### Preprocessing

I created a **custom preprocessing script for each model** to handle differences in formatting, structure and labelling. 

- **For traditional ML models** – More in-depth preprocessing, including tokenization, lemmatization, lowercasing and removing URLs and user mentions. The preprocessing for COVID-19 and ADR datasets differs slightly to fit the needs of each topic. For example, in ADR datasets I used a comprehensive drug list so that any detected drug name in the text was automatically labelled as \<DRUG\> .

- **For deep learning models** – Lighter preprocessing, mainly replacing URLs and user mentions while keeping most of the original text intact.

**Early challenges** 🤔❓

Reddit data was straightforward to collect but Twitter required careful handling due to stricter access terms.

---

➡️ **Next week’s plan**
* Train baseline Machine Learning models. 
