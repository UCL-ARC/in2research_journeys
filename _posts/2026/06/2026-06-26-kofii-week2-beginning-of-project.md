---
title: Week 2- Begun working on Eye segmentation and federated learning project
date: 2026-06-26
time: "15:30:00"
author: kofii
categories: ["Linux", "Git", "Python", "Learning", "Pytorch", "deeplab", "Model training"]
layout: post
---



### Highlights
- This week, I started to train the sample datasets on the Github repository (Mobious and openEDS data) on the local CPU device.
- I also perfored some data augmentation on these said datasets on the repo for training the model. This was done using the transformation functions to  easily resize and  rescale the images for effective training
- I researched a lightweight model to be able to handle training large datasets on the local CPU device. This led to me creating a new python file, importing the script from Pytorch, creating a new configuration file and  changing thhe various paths for the weights of the light-weight model to be stored.
- There were some issues with segmentation on the repo files so I had to create a new log on the repo to be solved by the creators. We later got it fixed by some suggestions from my suprevisors and created a new issue explaining how it thad been fixed for others to learn from.


### Setbacks
- The training of these very large datasets were meant to be trained on  GPU device and not a local CPU because of memory issues. So, I was only able to train about 10 samples from Mobious and 9 from openEDS before the model was trained without any faults hence not making it too efffective
- Implementing of lightweight model was slightly complicated as the datasets seemed to be written to accomodate UNet and segnet models. 
- All weights from UNet and Segnet are stored in one folder hence slightly distinguish between them. Will fix that and be done  with it next week

### Next Week's Plan
- Meet up with my supervisors to discuss my setback from earlier and derive a solution
- Start implementing Federated Learning in the project to protect patient's data
- Should complete training the lightweight model (deeplabv3) with openEDS and Mobious
- Start training all models with RTI-eyes dataset
