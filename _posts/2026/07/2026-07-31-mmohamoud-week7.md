---
title: Week 7 - Model Training + project merging   
date: 2026-07-31
time: "17:30"
author: mmohamoud
categories: ["U-Net", "RITnet","myriad", "Model","deep learning","training","merge"] # This is optional, list of categories that you want to add
layout: post
---

### Highlights

* This week, I successfully merged my work so far with Kofi’s work into one shared fork. This was an important step as it brought our progress together and made it easier to continue working from the same version of the project.
* I also began working on the RITnet model and tweaking it so that it can run on my prepared datasets. So far, I have had success getting it to work with the MOBIUS dataset locally and have a prepared job for it to run on myraid.
* I reran the UNet model and added extra metrics to the train_unet_with_openeds script. Previously, I was only able to view the average loss, but now I can begin recording proper segmentation metrics such as DICE, IoU etc which will be crucial for the benchmarking after training is doen.

### Challenges

* Issues with unzipping the RIT-eyes full dataset on myriad with the default Unzip tool despite being extracted with no issues when using the default file explorer unzip, resolved using 7-Zip.
* My fork had a broken commit history due to accidental rewriting, resolved by reforking and adding changed files.
* Issues with training RIT-eyes on UNet still due to corruption supposedly, have redownloaded the dataset and unzipped on myriad to see if it is an issue with the dataset or augementation.

#### Goals for Following Week

* Train RITnet / Deeplab on all the original + augmented batches for all 3 datasets.
* Begin working on poster and end of placement presentation.
* Begin benchmarking and analysing results / rerunning job with errors / poor results.