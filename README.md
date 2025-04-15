# Code-Temp-Repo
This is a template repo for new projects within perception and control system, especially when you need to work together with others. You are REQUIRED to use Github for code sharing, co-development, and project management. 

You are suggested to use this template to create a new repository for your project. [Here](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template) is how.

## Table of Contents

- [Required](#required)
- [Suggested](#suggested)
- [For project leader](#for-project-leader)
- [Repository structure](#structure)

## Required

- Formiliarize yourself with Github and the Branch-Based Workflow.
    - Github: Chapter 6, 7, and 8 of this [book](https://third-bit.com/py-rse/git-cmdline.html)
    - Branch-Based Workflow: to learn what and why we use branch-based workflow, watch this [video](https://www.youtube.com/watch?v=gW6dFpTMk8s)
- Well structure your code into relevant folders, you can create new folders, but you need to add and explain it in [Repository structure](#structure).
- Good documentation is required, not only for your teammates but also for yourself.
- **Follow the following steps to facilitate extensible and efficient collaboration.**
    1. Create a new issue. 
        - [Here](https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/creating-an-issue) is how.
        - Give this issue a number and a brief introduction in the name, e.g. `#1_pv_prediction_heuristic`. 
        - Project leader could assign this issue to your team member.
    2. Create a new branch.
        - Give the branch the same name as the related issue.
    3. Switch to and work on the new branch you created.
    4. Add, commit, push your new branch to the github (cloud).
    5. Create a pull request to merge your branch with the master branch.
        - The project leader will review your pull request before he merge it.

## Suggested

- Test your code before you push it to this repo. Why both and how? See the Test-Driven Development (TDD) and unit test session in [Code Development](#code-development).
    - Learn what is [Test-driven development](https://www.xenonstack.com/blog/test-driven-development-python)
        - For project leaders: save your trouble to review the code, and avoid one unnoticed change mess up the whole project.
        - For team members: help them know what exactly you want, and help them to validate their codes.
    - Unit test in Python
        - [Blog](https://machinelearningmastery.com/a-gentle-introduction-to-unit-testing-in-python/)
        - [Video](https://www.youtube.com/watch?v=6tNS--WetLI)
    - The project leader could define some test so that he/she does not need to go to the details of the developed code before merging it.
- It is not suggested to upload data file to this folder.

## For project leader

- Your job is to 
    - Divide the whole task into sub-tasks.
    - Clearly define what each sub-task is.
    - Think about how to check whether each sub-task is correctly implemented.
        - Test-driven development can help, if you do not want to review the code line by line.
- TODOs
    - Make sure everyone is on the same page.
    - Clearly let your team members know what you want from them.
    - The more strickly you follow the above workflow, the easier for you to manage the project.
    - The more detailed you define each sub-task and the interface between two members (e.g. the inputs, and outputs), like [this](/utils/gradientDescent.py), the easier it would be when you put every piece of the work together.
    - The larger the team you manage, the more strictly you need to follow the above workflow.

## Structure

``utils``: functions that will be used again and again

``data``: data collection, pre-processing, and evaluation

``src``: code for deployment

``unittests``: code for unit testing
