# Grounding Techniques for LLMs

This is the repository for the LinkedIn Learning course `Grounding Techniques for LLMs`. The full course is available from [LinkedIn Learning][lil-course-url].

![lil-thumbnail-url]

<p>Are you looking to learn more about large language models (LLMs)? Join instructor Denys Linkov as he explores hallucinations, their causes, the implications they have on the reliability and usability of LLMs, and how to mitigate structural and contextual inaccuracies to ensure high-quality, time-sensitive output. Develop practical techniques for addressing hallucinations, including few-shot learning, model fine-tuning, and templates for guiding LLM outputs. You'll also delve into more advanced topics like the chain of thought reasoning, retrieval-augmented generation, and model routing to enhance LLM performance. Test out your new skills along the way with real-world challenges that provide hands-on experience to solidify your learning. Whether you’re an AI researcher, a data scientist, or a tech enthusiast intrigued by the evolving capabilities of LLMs, this course offers valuable insights on navigating the complexities of AI with ease.</p><p>This course is integrated with GitHub Codespaces, an instant cloud developer environment that offers all the functionality of your favorite IDE without the need for any local machine setup. With GitHub Codespaces, you can get hands-on practice from any machine, at any time-all while using a tool that you'll likely encounter in the workplace. Check out the "Using GitHub Codespaces with this course" video to learn how to get started.</p>

_See the readme file in the main branch for updated instructions and information._

## Instructions

This repository has branches for each of the videos in the course. You can use the branch pop up menu in github to switch to a specific branch and take a look at the course at that stage, or you can add `/tree/BRANCH_NAME` to the URL to go to the branch you want to access.

## Branches

The branches are structured to correspond to the videos in the course. The naming convention is `CHAPTER#_MOVIE#`. As an example, the branch named `02_03` corresponds to the second chapter and the third video in that chapter.
Some branches will have a beginning and an end state. These are marked with the letters `b` for "beginning" and `e` for "end". The `b` branch contains the code as it is at the beginning of the movie. The `e` branch contains the code as it is at the end of the movie. The `main` branch holds the final state of the code when in the course.

When switching from one exercise files branch to the next after making changes to the files, you may get a message like this:

    error: Your local changes to the following files would be overwritten by checkout:        [files]
    Please commit your changes or stash them before you switch branches.
    Aborting

To resolve this issue:
Add changes to git using this command: git add .
Commit changes using this command: git commit -m "some message"

### Instructor

Denys Linkov

ML Lead at Voiceflow

Check out my other courses on [LinkedIn Learning](https://www.linkedin.com/learning/instructors/denys-linkov?u=104).

[0]: # "Replace these placeholder URLs with actual course URLs"
[lil-course-url]: https://www.linkedin.com/learning/grounding-techniques-for-llms
[lil-thumbnail-url]: https://media.licdn.com/dms/image/v2/D560DAQEN2aoK9FmRuw/learning-public-crop_675_1200/learning-public-crop_675_1200/0/1724282276424?e=2147483647&v=beta&t=F9TibZ0gmZ6gTAqKruZNc3SToibaHgGAsfQVXO4ie0w


N.T.:

# Fetching all branches to the codespace:

git pull --all
$ git pull --all
Fetching origin
Fetching upstream
remote: Enumerating objects: 156, done.
remote: Counting objects: 100% (156/156), done.
remote: Compressing objects: 100% (65/65), done.
remote: Total 153 (delta 82), reused 153 (delta 82), pack-reused 0 (from 0)
Receiving objects: 100% (153/153), 127.78 KiB | 4.91 MiB/s, done.
Resolving deltas: 100% (82/82), completed with 1 local object.
From https://github.com/LinkedInLearning/grounding-techniques-for-llms-3896093

- [new branch] 00_02 -> upstream/00_02
- [new branch] 01_03 -> upstream/01_03
- [new branch] 03_04 -> upstream/03_04
- [new branch] 03_06 -> upstream/03_06
- [new branch] 03_07 -> upstream/03_07
- [new branch] 03_08 -> upstream/03_08
- [new branch] 03_09 -> upstream/03_09
- [new branch] 04_02 -> upstream/04_02
- [new branch] 04_03 -> upstream/04_03
- [new branch] 04_04 -> upstream/04_04
- [new branch] 04_05 -> upstream/04_05
- [new branch] 04_06 -> upstream/04_06
- [new branch] 04_07 -> upstream/04_07
- [new branch] 04_08 -> upstream/04_08
- [new branch] 04_09 -> upstream/04_09
- [new branch] 04_10 -> upstream/04_10
- [new branch] main -> upstream/main
  Already up to date.

# As a result, we can list all (remote) branches:

$ git branch -a

- main
  remotes/origin/HEAD -> origin/main
  remotes/origin/main
  remotes/upstream/00_02
  remotes/upstream/01_03
  remotes/upstream/03_04
  remotes/upstream/03_06
  remotes/upstream/03_07
  remotes/upstream/03_08
  remotes/upstream/03_09
  remotes/upstream/04_02
  remotes/upstream/04_03
  remotes/upstream/04_04
  remotes/upstream/04_05
  remotes/upstream/04_06
  remotes/upstream/04_07
  remotes/upstream/04_08
  remotes/upstream/04_09
  remotes/upstream/04_10
  remotes/upstream/main

NOTE:  in local:
c:\SRC\Py\devprep\00_GOOGLEDEV\GroundingLLMs>git branch -a
* main
  remotes/origin/00_02
remotes/origin/01_03
remotes/origin/03_04
remotes/origin/03_06
remotes/origin/03_07
remotes/origin/03_08
remotes/origin/03_09
remotes/origin/04_02
remotes/origin/04_03
remotes/origin/04_04
remotes/origin/04_05
remotes/origin/04_06
remotes/origin/04_07
remotes/origin/04_08
remotes/origin/04_09
remotes/origin/04_10
remotes/origin/HEAD -> origin/main
remotes/origin/main

Scrolling across branches:

git branch     # list only local branches
git branch -a  # list all local and remote branches
git branch -r  # list all remote branches only

git switch BRANCH_NAME   # switch to an existing branch
git checkout BRANCH_NAME # switch to an existing branch

git switch -c new_branch_name  # create a new branch and switch to it
git checkout -b new_branch_name # create an new branch and swithc to it