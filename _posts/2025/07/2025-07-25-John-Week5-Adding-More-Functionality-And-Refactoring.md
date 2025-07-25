---
title: Week 5 - Adding More Functionality and Refactoring
date: 2025-07-25
time:"17:00"
author: john
categories: ["refactoring"]
layout: post
---

### Highlights

- Modularising functions used in the training file, ensuring reused functions are put into a seperate utility function library. Doing it this way improves code maintability and readability for collaborative development. The functions migrated include the function responsible for creating the data loaders, the one responsible for the training and validation loops, and the one responsible for writing the metrics and loss values to .json and .csv files.
- Adding functionality to load a pre-trained model into the training file, bypassing the training and validation loop and starting at the evaluation process. This is good to test how pretrained models perform on previously unseen test sets.

### This Week's Challenges

- One challenge faced was ensuring that when the training and validation loops were migrated, their functionality. This taught me that when primative types are passed into functions, Python creates local copies so any modifications don't affect the original variables. However, since objects like the `model` and `optimizer` are passed into functions as references to objects in memory, any modifications in the functions affect the original object. This realisation helped me solve a ZeroDivisionError. 

### Next Week's Plan

- Create a 1-page summary of my work to present to project stakeholders.
- Run inference bash script to see how model handles unseen data.
- Plot loss and accuracy graphs to visualise model performance.
