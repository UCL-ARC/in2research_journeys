---
title: Week 6 - Improving Plotting Scripts
date: 2025-08-01
time: "15:00"
author: john
categories: ["graphs", "matplotlib"]
layout: post
---

### Highlights

- Added further instructions to documentation for when people download our model from Hugging Face.
- In preperation for my talk in the Tuesday Social in a couple weeks time, I created a draft powerpoint that I've shared with Miguel and Stephen. In our call, we discussed how to improve it, such as fixing the formatting, using QR codes instead of web links, and splitting my contributions over multiple slides instead of a single slide.
- Enabled the inferencing script, a script that produces plots showing how the model segments an image of an eye into different sections, to work on non-gpu machines.
- Added additional functionality to plot_losses.py and plot_performance.py. These files are now able to take a list of loss value and performance metric files and plot them on the same graph. This is helpful when comparing the performance of more than one model. Plotting the loss values is especially useful since we can see after which epoch a model demonstrates overfitting behaviour.

### This Week's Challenges
- Debugging why I couldn't load in models stored in repositories cloned from Huggin Face. After doing some googling, I figured out that instead of the model weights being downloaded when the repo was cloned, instead a pointer to the file containing the model weights was being used instead. To fix this, I had to download the raw file from the Hugging Face repo. This step is reflected in the docs.

### Next Week's Plan
