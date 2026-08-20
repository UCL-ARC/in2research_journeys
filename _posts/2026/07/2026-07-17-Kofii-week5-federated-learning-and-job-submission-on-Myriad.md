---
title: Week 5- Federated Learning and job submission on Myriad
date: 2026-07-17
time: "16:20:00"
author: kofii
categories: ["Linux", "Git", "Python", "Federated Learning",  "UNet", "model training", "OpenEDS", "Mobious", "RIT-Eyes", "myriad", "RDSS" ]
layout: post
---



### Highlights
- I finally gained access to Myriad. A HPC that enables us to use the GPU Nodes to submit jobs on it. Ruaridh and Zakaria gave me Mohamed and I an onbarding into how Myriad works, how to submit a job, how to track a job, how to use Scratch, a temporary storage allocated for Myriad and everything. This access is a huge step in my project as I will not have to run huge scripts on my local CPU machine and run into segmentation faults. I have submitted my first job script training UNet on the full datasets of Mobious, OpenEDS and RIT-Eyes respectively for it to run over the weekend
- I had an issue with my local computer's storage as I had to download these massive datasets locally. So, even after gaining access to Myriad, my storage space makes the laptop run slower. We discussed this with David who suggested to Ruarish, Miguel and Zakaria to use RDSS to store our datasets. RDSS is a remote storage for ARC that allocates 1TB of storage pfr every project. Miguel made a request and we now have access to RDSS. I am currently transferring all the datasets to it, access and modify them there from now on and free up some space on my computer so I can run tasks effectively
- During our 1:1s, my supervisors and I decided it was time to start merging Mo and I's code together. It has been agreed to do that next week just to make sure my code running on Myriad currently works and that I am merging working code Mo's branch before merging it to Main. This is a huge step as it shows we've done enough work to finally contribute to the repo. I have also modified my code based off the reviews I received from my supervisors in our last code reviews. This makes it more robust and effective
- Now that I have two fully functional models that effectively train at least 2 datasets, will be 3 by next week. I was given a brief introduction to the implementation of Federated Learning during our 1:1s. Will hopefully start with that next week

### Setbacks
- Only setback has to do with RDSS and Myriad. It seems like we don't have permission to modify the files on RDSS in myriad. It can be accessed, but not modified hence Myriad does not find the path when given to it for training. This means I have to manually move all the massive datasets from RDSS to Scratch which could take at least 2 days.

### Next Week's Plan
- Get started on Federated Learning after UNet is done running on Myriad over the weekend
- During our project meeting, start merging my code into Mo's branch, handling merge conflicts together
- If first two points are completed on time, implement a federated inference script to demonstrate optimised results during ARC Forum presentation and poster
