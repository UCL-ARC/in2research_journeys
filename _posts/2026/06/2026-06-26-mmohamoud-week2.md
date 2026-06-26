---
title: Week 2- Producing preprocessing package for image segmentation 
date: 2026-06-26
time: "17:30"
author: mmohamoud
categories: ["Augmentation", "Python", "Preprocessing","Research","Pytorch"] # This is optional, list of categories that you want to add
layout: post
---

### Highlights

* This week, I developed a simple preprocessing and augmentation package and tested on the sample images in the READY repository along with the MOBIUS dataset. The package can resize images and create augmented versions such as horizontal flips, vertical flips and grayscale.

* After receiving feedback, I improved the package by adding command-line arguments through `argparse` to make it more tailorable. The code also uses `Pillow` for image processing and `pathlib` for cleaner file handling, allowing the user to choose the image folder, mask folder, output folder, resize dimensions and sample limit without editing the code directly.

* I began researching and reading more on OpenEDS, RITnet and OcularSeg to understand eye segmentation datasets, mask preparation, segmentation classes and useful augmentations for U-Net training, such as CLAHE, elastic transforms and gamma correction.

### Challenges

* A key challenge was ensuring that my package was a good reusable preprocessing package, rather than just writing a script that works for one folder on my own computer. I had to think more carefully about how another user could run the package on their own device and the issues with my first draft and how to pivot.

* I also had to do further research into data augmentation for image segmentation tasks. I needed to understand which transformations should be applied to both images and masks, such as flips and rotations, and which transformations should only affect images, such as colour changes or grayscale conversion.

* I faced some practical issues while working locally, including storage issues mainly and issues with code not producing intended outputs or no outputs spent a lot of time debugging code.

* ☀️🔥😰

#### Goals for Following Week

* Improve the preprocessing package so it can be tested more clearly across MOBIUS, OpenEDS and RIT-Eyes style datasets as well as also be used as a general reusable package for image segmentation tasks, while keeping the code simple, reusable and easy for another user to run.
* Begin connecting the preprocessing and augmentation work to the training pipeline.
* Add additional augmentation techniques to allow for a more flexible package and for models to be trained on a wider range of images variability.