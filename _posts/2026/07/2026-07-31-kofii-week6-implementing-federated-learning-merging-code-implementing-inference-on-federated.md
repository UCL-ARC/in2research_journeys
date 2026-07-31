---
title: Week 5 - Implementing Federated Learning, merging code and implementing inference on federated learning for demonstarting output on poster 
date: 2026-07-31
time: "16:30:00"
author: kofii
categories: ["Linux", "Git", "Python", "Federated Learning", "Myriad", "UNet", "Code merging", "Merge conflicts", "Github", "Code reviews"]
layout: post
---



### Highlights
- From my previous blog post, I left Myriad to run on training UNet with all the datasets. It run without errors so my code had been approved for merging with Mo's branch and then after further review, we both merge it into the main branch. It was suggested I merge my code into Mo's branch first as he made least amount of changes to files compared to me. There were so many merge conflicts due to data path cdifferences, his preprocessing files, different styles of writing code, to name a few. Ruaridh, Mo and I sat together and resolved all those conflicts together. It was approximately 163 merge conflict files.
- After resolving these merge conflicts, I submitted the merge for review and accidentally pushed all the code to main, skipping review. This was about 101,000 lines of code which was not ideal for quality of code. Thanfully, Miguel was able to revert all those changes and it made me a bit worrried as this could have been a huge issue. Ruaridh and Zakaria were really helpful and assured me that it was alright to make such mistakes and that I am in this placement to learn after all. I am just going to be extra careful from now on to not repeat such mistakes
- I have implemented federated learning script for all three datasets. I have unfortunately encountered so many errors and have had to submit multiple jobs on Myriad. As at now, I can't tell whether my final job works without errors as it takes days to finally get results due to the size of these clients. Hopefully I can get it all sorted by next week, finalise everything, clean up code and then have enough results for the ARC Forum presentation and poster presentation


### Setbacks
- For the implementation of federated learning, it take a really long time to run on Myriad. Sometimes, a job may take 3 days before it finally compiles, and then I end up getting an erro, fix that error and run again for another 3 days maximum. This makes it really difficult to track what I need to do quickly. To somewhat fix this, I have decided to delete all datasets from my computer and then train a small set of datasets locally to find out if it runs without errors or notbefore submitting to Myriad

### Next Week's Plan
- Pair programming with Mo to clean up code, add additional functionalities and code together on the new main branch 
- Code reviews, 1:1s and Project meetings, and mock presentation to show findings and results
- Finish up inference on federated Learning
