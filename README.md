# in2research_journeys

## Contributing to this repository

1. Fork the repository (click on the Fork button on the top right corner)
2. Clone the repository locally. Using VSCode, open a new window, make sure there's no any folder open (File, close folder), go to the "Source Control" menu, and click "Clone Repository". In the top menu you could filter typing `in2research_journey`. Choose the one that shows your user name.

  - Only the first time, we want to configure main to track the upstream repository,
    running this command on VS Code terminal (in Windows make sure you've got gitbash):
    ```
    git remote add upstream https://github.com/UCL-ARC/in2research_journeys.git
	git pull --set-upstream upstream main
    ```

3. Create a new branch, clicking in the lower bottom corner where it says `main` and give it a name. You will have to create new branches for each post. You can name them as `<your-initials>/week<number>`.
4. Modify/Add files as shown below, stage and commit them
5. Push them to your fork.
6. Visit the upstream repository (i.e., `UCL-ARC/in2research_journeys`) and you will see a yellow banner in the top asking whether you want to open a Pull-Request. Create one pull request.
7. The Pull request will be reviewed and merged when any comment has been taken care of.

For the second and consecutive blog posts you'll need to update the main from upstream. To do so, you can change back to `main` and pull the repository. Then you continue from step 3.


## Adding yourself as an author

Create a new file under the `_authors` directory named as `short_name.md` where `short_name` is the same that the `short_name` tag in the example below.

```md
---
short_name: davidps
name: David PS
project: HPC
year: 2025
github: dpshelio
---

David is an astrophysicist interested in brains.

```


## Adding a new post

Create a new file with the following format `YYYY-MM-DD-authorname-title.md` under the `_posts/yyyy/mm/` directory.

The file should look like

```md
---
title: Your Title
date: 2025-06-11
time: "15:30:00"
author: your-short-author-name
categories: ["learning", "python", "introduction"] # This is optional, list of categories that you want to add
layout: post
---

Here you write your content on markdown. If you want to add an image, you can add them under
`images/yyyy/mm` and link them as:

![](/in2research_journeys/images/yyyy/mm/image-file.jpg)

or if you want to have control of its size, using HTML format:

<img height="200px" src="/in2research_journeys/images/yyyy/mm/image-file.jpg" />
```
