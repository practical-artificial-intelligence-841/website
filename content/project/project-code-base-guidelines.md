---
title: Project Codebase Guidelines
weight: 4
---

## Getting Started
- GitHub org has empty repositories, named **project-m#-team#** 

- **Team member 1:** Creates initial project repo with empty README.md. Locally, in the COMP 741/841 directory, create **project** subdirectory 
    - **mkdir project** 
    - **cd project** 
    - **touch README.md** 
    - **git init**       <---- create git repo for the project working directory 
    - **git remote add origin [remote-repo-URL]**    
    - **git add README.md**	<-- stage or prepare for commit README.md 

    - **git commit -m 'create README.md'** 

    - Check that current branch is **main** 
        - **git branch -a**  <-- list all branches, local and remote 

    - If it's **master** do the following 
        - **git branch -m main**     <-- rename current active branch master to main 
    - **git push origin main**

## Codebase Structure Setup
- The **project** root directory has: 
    - **src** directory, where the source code files reside.  
    - **README.md, HOWTO.md, and CHANGELOG.md** required files. 

- Other directories in the root directory include: 
    - **resources**- has the codebase from other projects that are the basis of the team project 
        - Can be organized in subdirectories if multiple sources are used. 
        - Find good names for the subdirectories  
    - **docs** - has PROPOSAL.md, DESIGN.md, REPORT.md, project presentation, and other documentation files 
    - **data**  

- There might be other directories, depending on the project. 
- Team members switch roles to create a minimal codebase structure 
    - Team member 2 
        - Create minimal structure of the codebase:  
            - **src** directory, empty **md** files 
        - Add changes to version control and commit history 
            - git add . 
            - git commit -m 'create initial project structure' 
            - **git push origin main** 

    - Team member 1 
        - **git pull origin main** 

## Codebase Development
- Use GitHub project tool (both table and board view) to document project management work 

- Use **feature-branch git workflow**
    - Individual contributions of team members are documented on **branches** they create do their share of work 
        - Do NOT remove the branches: they document individual contributions of team members 
        - Development work on a branch MUST have meaningful **commit** messages 

- ONLY local branches are pushed to the remote, NOT **main** branch 
- After pushing a branch, team member opens a **pull request** with information about 
    - What the branch brings to the project: informative description 
    - Who’s assigned to review the work (the other team member) 
    - Which project the pull request belong to 

- The branch reviewer does one of the following: 
    - approval, changes, or rejection of the pull request 

- When the pull request is approved, the team member merges it into **main**   

