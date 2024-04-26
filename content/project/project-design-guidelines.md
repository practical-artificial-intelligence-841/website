---
title: Project Design Guidelines
weight: 3
---

## Content and Organization

### 1. AI System Overview

The AI system overview addresses these three questions: 

1. What **type of AI system** does your team investigate? 

    - Briefly summarize what the project type (not your particular AI system) is about.  

2. What **AI system** has the team selected from publicly available sources to exemplify the type of project under investigation?  

3. What **sources of information** has your team used to learn and conduct the project work?

To answer questions 2 and 3 above:
- Briefly describe the purpose of the selected AI system 

- List and analyze the credibility of the sources you have selected. These sources may include (but are not limited to): 

    - implementation code examples 

    - codebase remote repositories 

    - datasets 

    - pseudocode of the system's algorithms 

    - sites hosting the actual dataset (e.g., UNH academic integrity web page). 

Properly cite ALL the sources described in this section. See the References section for more information. 

### 2. Relevant Theoretical Background
The central question of this section is: 

- What **content knowledge** (theories and concepts) are needed to understand what your AI system does and how it works. 

Two elements narrow down the content knowledge relevant to your AI system: 

- The **type of project** your system represents  

- The AI system you've selected. 

Start with the more general context of the **type of project**. Take into account what's specific to your AI system to include relevant theoretical concepts. 

 
Properly cite ALL the sources from which you use content in writing this section.  

- See the References section for more information. 

### 3. AI System Development and Evaluation
- Review the objectives of the project type of your AI system (see the Appendix) 

- Apply each objective of the project type to your AI system development and evaluation 

- Describe each objective in the **very specific terms of your AI system** development and evaluation.  
    - The focus of this description is on **practical knowledge**: tools, platforms, APIs, libraries, and data sets needed to develop and evaluation of the AI system. 

### 4. Risks Exploration
- What **risks** might be posed by the AI system development, evalaution, and use? 
- Describe potential risks guided by the following resources:
    - The Communications of the ACM article by Esther Shein on Governments Setting Limits on AI. 
    - [Microsoft Aether Data Documentation template](https://www.microsoft.com/en-us/research/uploads/prod/2022/07/aether-datadoc-082522.pdf)

### 5. Project Milestones and Deliverables
Including this week, the team has 5 weeks to complete the codebase and project report (due **December 18, midnight**).  

- Create five subsections corresponding to the five weeks of the project.  

- Each subsection details the following 

    - Project development tasks aligned with the AI system development objectives 

    - Who is responsible for each task 

    - What each task will produce. 

Properly cite ALL the sources from which you use content in writing this section.  

- See the References section for more information. 

### 6. References
All the sources selected for the project study must be: 

- Included in the team's Zotero group library 

- Listed in the References section 

- Written in the reference style used in the reading notes.  

Citation style is (Author name(s), year). 

## Other Considerations - All or Nothing
The following requirements must be met in order to accept and consider your submission. Otherwise, there is no credit for this submission. 

### Equitable assignment of writing tasks
Team members collaborate closely on writing all the sections of the design document.  
- Add the names of both team members when team members contributed equally to a section or subsection. 

- Distinguish between primary author and reviewer when one of the team members took the lead on a section/subsection and the other team members provided assistance.  

Failing to provide clear attribution to the writing assignments results in **no credit** for the submission.  
 
### Organization and Formatting
- At the top of the design document have a title section that includes: 

    - Name of the document 

    - Authors 

    - Date.  

- Use ### (level 3) Markdown for the title and normal text for authors and date. 

- Structure the design document in 6 sections as described above.  

- Use #### (level 4) Markdown for the section headings.  

- In general, use paragraph style in writing the design sections 1, 2, 3, and 4. 

- Include bulleted lists ONLY inside paragraphs when appropriate.  

- The length of the design in PDF form is 3-4 pages. 

Failing to meet the organization and formatting requirements results in **no credit** for the submission. 

### Submission
- DESIGN.md in **docs** directory. Last commit before the deadline 

- PDF version uploaded to Canvas before the deadline.  
Failing to meet the submission deadline results in **no credit** for the design document assignment.  

Time extensions are not considered if requested after the deadline. Make plans to commit DESIGN.md changes often and have PDF versions of the drafts of DESIGN.md uploaded to Canvas as early as Monday noon time.

## Project Types
### Neural network classification/regression
- Find a clean classic dataset (from the TensorFlow dataset https://www.tensorflow.org/datasets  or Sklearn toy datasets https://scikit-learn.org/stable/datasets/toy_dataset.html) 

- Load the data presplit for test 

- Design the supervised learning model 

- Train the neural network so that it can correctly classify the test data set 

- Overfit the neural network 

- Graph the model performance as it overfits the neural network 

    - How does the model score on the test data set as it continues to train? 

    - How does the model score on the train data set (loss, accuracy) as it continues to train? 

### Search
- Study and evaluate search algorithms based on four types of AI search: 

    - Uninformed search: depth-first search, breadth-first search, iterative deepening, etc. 

    - Informed search: Best first search, greedy search, A* 

    - Local search: hill climbing and its variants 

    - Adversarial search: mini-max, alpha-beta pruning, Monte Carlo tree search 

- Select appropriate problem(s) to be solved with the AI search algorithms you are studying 

- Find high-quality open-source algorithm implementations of the algorithms that solve the chosen problems 

- Demonstrate and evaluate the algorithm's efficiency (time efficiency, space efficiency) on various inputs

### Large language model fine-tuning 
- Use Hugging Face pre-trained transformer-based BLOOM (BigScience Large Open-science Open-access Multilingual Language Model) large language model 

- Prepare dataset 

    - Scrape data source into a plain text or CSV file (either manually or using automated scraping with BeautifulSoup, for example) 

        - Example of data source: academic integrity policy 

    - Separate content of text file into sequences (sentences) represented on separate lines (rows) to train the model on 

    - Transform the data set into a Python list or dataframe (either manually by creating the content of the data structure, or automaticlly using Python libraries) 

- Download the BLOOM model  

- Fine-tune and train the model on the selected dataset 

- Evaluate performance using question-answer format 

- Use WebUI https://github.com/oobabooga/text-generation-webui 

### Constraint programming (CP)
- Decide the type of problem that the constraint solver will solve: 

    - Optimization problem, such as the assignment problem or scheduling problem 

    - Puzzles, such as cryptarithmetic puzzle, Sudoku, crossword puzzle, etc.  

- Find examples of constraint-based representations of the problem 

- Design and implement a constraint solver using two Google OR Tools constraint optimizaiton frame 

    - CP-SAT solver 

    - CP traditional solver 

- Evaluate and compare performances of the two implementations 

### Fine-tuning object detection
- Find a suitable Kaggle dataset for the class you want to train on 

- Familiarize yourself with LabelMe (an open-source label annotation tool) http://labelme.csail.mit.edu/Release3.0/ and https://github.com/wkentaro/labelme  

- Install labelme and use it to create JSON labels 

    - These labels are in the same format as those provided in Lab 6 

- Run labelme2coco to create the COCO train JSON (similar to Lab 6) 

- Evaluate performance on reserved test images  

### Evaluation of object detection
- Examine COCO web site and determine what COCO class(es) you want to evaluate (e.g., license plate) 

- Find a new dataset from Kaggle (chosen wisely) featuring the classes you want to evaluate (see lab 6 questions on analyzing the dataset) 

- Run an evaluation (by hand unless you write an evaluation script, see lab7 for details on displaying predictions) 

- Record performance 

- Compare performance with baselines in the Detectron2 Model Zoo 

    - Manually through image annotations 

    - Through programming (based on lab 6 setup.sh script applied to testing data) 

        - Note: Models in the Detectron2 Model Zoo are measured by “box AP” or ‘box average precision,’ or how much of the prediction bounding box overlaps the actual bounding box 

        - See automated evaluation script - https://github.com/facebookresearch/detectron2/blob/main/detectron2/evaluation/coco_evaluation.py 

- Interpret differences in performance by comparing datasets (manually) 

AWS. 2023. “What Is Deep Learning? - Deep Learning Explained - AWS.” Amazon Web Services, Inc. 2023. https://aws.amazon.com/what-is/deep-learning/. 

 



