---
title: Week 6 – Model Interpretability & Explainability
date: 2025-07-25
time: "11:30"
author: hirraa
categories: ["NLP", "XAI", "Interpretability"]
layout: post
---

This week I finalised the performance results for both the machine learning baselines and the deep learning models. I then applied explainability techniques to the models with top metrics using LIME (Local Interpretable Model-Agnostic Explanations) and 
SHAP (SHapley Additive exPlanations) to understand why they predict what they do and which words most influence each class.

I generated:
 * Instance level explanations with LIME 🍋‍🟩 and SHAP 🔴 to inspect individual predictions.
 * Global views with SHAP to see overall feature/token influence.
 * Token importance plots (top‑15) for each task: positive vs. negative on the COVID‑19 classifier, and ADR vs. non‑ADR on the ADR classifier.
 * SHAP force plots to visualise how specific tokens push predictions toward each class 📊

---

**Challenges** 🤔❓ 

* Computing SHAP values across the dataset takes significantly longer than instance level LIME and standard evaluation, especially on transformer models⏳

---

**Next steps** ➡️ 

* Data visualisations and start writing up the findings ✍️
