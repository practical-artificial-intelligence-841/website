---
title: Project Proposal Guidelines
weight: 1
---

## Overview
The purpose of the **team project** is to investigate and showcase the applicability of symbolic and neural AI approaches. You'll collaborate with a peer to propose, design, document, and showcase your investigation.  Project artifacts include a project proposal, project design, codebase, a final report, and a demo (see Course Syllabus).  

The **project proposal** addresses the following aspects of the team project: 

1. What **type of AI system** will the team investigate?  

2. What **AI system** has the team selected from publicly available sources to exemplify the type of system under investigation? 

3. What **content knowledge** (theories and concepts) are needed to *understand* what the AI system does and how it works? 

4. What **practical knowledge: tools, platforms, APIs, libraries, and data sets** are needed to *develop* the AI system?  

5. What **risks** might be posed by the AI system development and use? How are the risks mitigated? Consider the following issues:
    1. Safety and security
    2. Protection of data privacy
    3. Protextion against algorithmi discrimination
    4. Transparency and explanation

6. **References:** What trustworthy and publicly available materials and resources inform and guide the project work of the team? 


## Team Contributions
Team members collaborate to: 

- Explore and select an **AI system example** of the assigned **AI system type** using trustworthy and publicly available materials and resources (to address #1 and #2 above)

- Assemble relevant **references** from the assigned readings, other references made available in the course notes, Wikipedia, and other adequate sources (to address #6 above)
    - Set up a team project Zotero libray
    - Add the references to the team project Zotero library
    - List the references in Section 6 of the proposal.  

## Individual Contributions
Team members decide to equitably divide the task of writing sections 3, 4, and 5.  

- Determine the team member who's the lead author and the team member who's the reviewer for the following questions: 

    - Member 1: Questions 3 and 5.1 and 5.2

    - Member 2: Questions 4 and 5.3 and 5.4

- Include the **names** and **roles** along with the text of the question in the proposal.

## Development
The project proposal can be developed through direct, real-time collaboration between team members.  


- On the **main** branch, create **docs** directory. In this folder, create **PROPOSAL.md** . 

- Team members collaborate to write their sections and review the collaborator’s sections according to the planned writing assignments. 

- When development is done, **main** branch Is pushed to the remote.  

## Organization and Formatting
- At the top of the proposal have a title section that includes: 

    - Title of the project, authors, and date.  

    - Use ### (level 3) Markdown for the title 

    - Normal text for authrs and date. 

- Structure the proposal document in 6 sections, corresponding to the aspects that the proposal addresses.  

- The names of the section headings should be suggestive of what the section is about. 

- Use #### (level 4) Markdown for the section headings.  

- Use paragraph style in writing the section content. 

- The length of the proposal in PDF form is 3-4 pages. 


## Submission
- PROPOSAL.md in **docs** directory 

- PDF version of the proposal submitted by each team member in Canvas. 

## Optional: Feature-branch Development Workflow

- The team lead creates a **docs** directory with **PROPOSAL.md** file in it on the **main** branch 

- Each contributor creates a branch based off **main**, in which they draft the sections assigned to them. 

    - For example, Mihaela gets started with mihaela-1-proposal. Her partner, Ann, does her work on **ann-1-proposal**.  
- During drafting, the contributor commits changes to their branch 

- When done, the contributor does the following: 

    - Push their OWN branch to the remote 

        - For example: 	**push origin mihaela-1-proposal** 

        - This assumes that the **origin** is the location of the course remote repo 

    - In GitHub, the team member who pushed their branch 

        - Open a **pull request** to ask that their branch be “pulled” into **main** branch 

        - Assign the review of the request to the other team member (e.g., Ann) 
- When the reviewer approves the request, the contributor does the merging of their branch into **main** in GitHub 

- There might be merging conflicts if another team member has already done the merging of their changes. In that case, the conflicts are resolved through real-time, direct communication between the authors (in GitHub or locally) 