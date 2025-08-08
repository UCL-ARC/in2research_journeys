---
title: Week 5 – Model Testing & Fine-Tuning
date: 2025-07-21
time: "11:30"
author: hirraa
categories: ["NLP", "Deep Learning", "Fine-Tuning"]
layout: post
---

This week I carried on developing my deep learning pipelines and explored additional transformer architectures , including **DeBERTa**, which showed stronger performance than **BERT** 📈. It improves upon **RoBERTa** by using *Disentangled Attention*, where the model separates content and position information, allowing it to capture relationships between words more effectively.  

We decided the best evaluation strategy is to test all machine learning and deep learning models on each dataset individually, then combine the datasets and test again. For all methods, I’m using an **80/20 train–test split** to keep comparisons consistent.  

I then fine-tuned the models, lowering learning rates for smaller datasets to minimise the risk of unstable weight updates
and preserve learned representations, enabling more stable convergence. Where class imbalance was present, I applied class-weight balancing to help the models learn equally from minority and majority classes. 
I also optimised the number of training epochs to balance training efficiency with generalisation performance ⚙️🔬.

---

➡️ **Next steps:** Apply explainability techniques to better understand model decision making and identify which tokens contribute most to predictions.  
