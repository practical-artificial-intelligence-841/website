---
title: Git Feature Branch Workflow
weight: 6
---

## References
Atlassian Tutorials. 2023. Git Feature Branch Workflow. https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow 

## Workflow Description
- The **main** branch represents the official project history 

- Developers create a new branch every time they start work on a new feature 

    - Name your feature branch with your first name, followed by dash -, and very brief and descriptive name of the high-level focus of the branch.  

    - All feature branches are created off the latest code of a project, which is maintained by the **main** branch 

- Feature **branches** (NOT **main** branch) are pushed to the remote repository in order to be shared with the other developers without touching the official code.  

    - Use **push** command with EXPLICIT arguments, e.g.,  

        - **push origin mihaela-read-data**  

## Workflow Steps

#### Locally, on your machine
1. Switch to **main** branch, copy what has been added to the main branch from other branches, and reset local copy of **main** to match the latest remote main copy 

    - **git checkout main**	<-- Active branch becomes **main** 

    - **git fetch origin**	<-- Copy to the local remote **all new changes** from the remote **origin** 

    - **git reset --hard origin/main**	<-- local main is reset to its latest commit on origin 
 

2. Create the **new branch** based on the updated local main 

    - **git checkout –b mihaela-1-feature-x main** 

        - Be explicit about **main** being the branch off which you create your new branch.  

    - **git branch -a**    <-- list all branches 

3. Develop code on the new branch by editing files, “staging” them (**add** to prepare them for **commit**), and committing changes 

    - **git status** 

    - **git add <some files>** 

    - **git commit –m ‘... meaningful message... ‘** 

 
4. Push **feature branch** to the remote  

    - **git push origin mihaela-1-feature-x**

#### Remotely, on Github
5. Get feedback on the new feature branch 

    - Open a pull request in GitHub 

    - Fill in pull request information 

        - Name of the assigned reviewer (your project member) 

        - Name of the project 
 

6. Reviewer examines what has been committed 

    - Add comments specific to lines in the files of the commit 

    - Decides to approve, reject, or request changes based on comments  

#### Locally, Review
7. Developer resolves feedback LOCALLY 

8. Commits the new changes and push again the branch.  

#### Remotely, Review
9. Developer’s updates appear in the pull request. Reviewing continues until the reviewer approves the changes.  

10. When the pull request is approved 

    - Developer merges their branch into main and resolve any merge conflicts 