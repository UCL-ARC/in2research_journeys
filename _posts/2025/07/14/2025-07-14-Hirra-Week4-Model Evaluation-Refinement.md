---
title: Week 4 – Model Evaluation & Refinement
date: 2025-07-14
time: "09:00"
author: hirraa
categories: ["NLP", "machine learning", "deep learning" , "hyperparameter tuning"]
layout: post
---

This week I tested my machine learning models by merging all 3 social‑media datasets to create a more diverse train–validation split and assess how well they handle domain shifts. 

I then ran my deep learning pipeline, using transformer models like BERT BASE and RoBERTa, through both training and testing phases, logging key metrics (F1, ROC‑AUC, precision, recall, accuracy) 📊. I also compared these results against our baseline machine learning models to see which produced the best result.

Challenge: the larger transformer models are taking significantly longer to train and evaluate ⏳

➡️ Next steps: I’ll experiment with smarter batch size schedules (and possibly mixed‑precision training) to speed up training and then fine‑tune hyperparameters based on the newly collected results.
