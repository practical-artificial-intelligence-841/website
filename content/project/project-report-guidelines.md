---
title: Project Report Guidelines
weight: 6
---

## Content and Organization 

### 1. AI System Overview (1 1/2 -2 pages) 

The AI system overview addresses these three questions: 

1. What **type of AI system** does your team investigate? 
    - Identify one of the seven project types outlined in the Appendix of this handout. 
    - Briefly describe the project type (NOT your particular AI system). 

2. What **AI system** has the team selected?  
    - Briefly describe the **selected AI system**, including the problem/issue it addresses/solves.  
    - Cite appropriate references, as appropriate, in your description. 

3. What **sources of information** has your team used to get started?  
    - These are NOT all the sources you have in the Reference list. They are the very initial sources that: 
        - Informed your decision for the AI system you've selected.  
        - Provided sufficient information to give you a solid, clear starting point.  
    - Briefly describe (and CITE in the **References** section) ALL the sources that **guided the selection of your AI system**. These sources may include:
        - Technical/documentation materials made available by tech companies, educational institutions, media outlets, publication venues, or other credible sources of information 
        - Repositories of source code, examples of implementation techniques, algorithm descriptions 
        - Datasets, data descriptions, data files, problem instance examples, etc. 
        - Other sources relevant to your AI system. 
    - Analyze the **credibility of the sources** you have selected, based on available information about: 
        - Author/owner of the content of the source 
        - Date, license, provenance of the content 
        - Public recognition or prestige of the outline/venue/publication 
    
### 2. Relevant Theoretical Background (1 page) 
The central question of this section about the **content knowledge** (theories and concepts) that are needed to understand and explain:  
- What your AI system does and  
- How the system works. 

Consider the following approach: 
- Introduce the key concepts and techniques that are essential to the understanding and development of **your AI system**.
- Organize the content of the section as follows: 
    - Start with the more general context of the type of project of your AI system. 
    - Narrow down the content knowledge to what is relevant and specific to your system. 
- Cite appropriate references, as appropriate.   

### 3. AI System Development and Evaluation (1-2 page) 

The purpose of this section is to describe the development and evaluation of your AI system. 
- Review the objectives of the project type of your AI system (see the Appendix) 
- Apply each objective of the project type to the development and evaluation of your AI system. 
- Describe each objective in the **very specific terms of your AI system** development and evaluation.  

### 4. Project Management (1-2 pages) 
Document the entire process of managing the project activities.  
- Organized the section into five subsections that correspond to the five weeks of the project.  
- Evidence of the completed activities is also available on the project board in GitHub. 
- Each subsection details the tasks team members worked on.  
- For each task, make clear who did what and what exactly was achieved (concrete deliverable or artifact).  

### 5. References 
All the sources selected for the project study must be included in the team's Zotero group library and in this section.  
- References must be written in the reference style used in the reading notes.  
- ALL references **must be cited** in the text using the citation style of Author name(s), Year.  

### 6. Appendix (Optional unless Required by Project Type) 
Figures, charts, sample data, and other visuals are included in the report's Appendix section. They must have numbered captions and must be cited in the sections for which they provide useful information. To cite a figure/chart/table, use the notation Figure (Table) #, where # is the number of the figure/table.  

## Other Considerations 
The following requirements must also be met in order to accept and consider your submission.  

### Equitable assignment of writing tasks - All or Nothing 
Team members collaborate closely on writing **ALL the sections** of the report document. Note: The division of labor works for 2-member teams. 

To divide the writing of each section between team members:  
- Determine the PARTS of the section for which there is a PRIMARY author and a REVIEWER. A PART is a subsection with a subheading. 
- The PRIMARY author takes the lead of writing the **subsection**, while the REVIEWER provides assistance.  
- Authorship and role information MUST be included immediately **under the heading of the subsection**.  
- It is entirely the responsibility of each team member to carry out their assigned writing tasks.  

Failing to provide clear attribution to the writing assignments results in **no credit** for the submission.

### Organization and Formatting - All or Nothing 
- At the top of the report document have a title section that includes: 
    - Name of AI system 
    - Type the document (Project Report) 
    - Course number/name and course instructor 
    - Author names 
    - Date  
- Use ### (level 3) Markdown for the title and normal text for document type, authors, and date. 
- Structure the report document in 5 sections as described above.  
- Use #### (level 4) Markdown for the section headings.  
- Use ##### (level 5) Markdown for subsection headings in each section.  

### Length - All or Nothing 
The length of the report in PDF form is **4 1/2 to 6 pages WITHOUT counting:** 
- Title section 
- References section 
- Appendix section

### Submission - All or Nothing 
- REPORT.md in **docs** directory. Last commit before the deadline, Monday, Dec 18th. 
- PDF version uploaded to Canvas before the deadline.  

There is **NO** time extension for the project report.  

### Writing Style and Content 
- In general, use paragraph style in writing the report sections 1, 2, 3, and 4. 
- Address all the requirements of each section.  
- Have well-constructed sentences.  
- If you have bulleted lists, include them inside paragraphs when appropriate. 

### Figures and Tables 
- If you use figures and tables 
    - Captions must describe what the figure/table is about. 
    - Format: Figure # (or Table #), where # is the number of the figure and table., followed by the caption text.  
    - All figures/tables in the Appendix MUST be cited in the report, in places where figures/tables provide a good illustration of what you are saying in the report.   

- If the figure/table is NOT authored by you, then you must add citation.  
    - There must be a reference item in the References section for this citation. 
    - The reference must be easily identifiable. 

## Appendix: Project Types 

### Regression and Classification
- Find a clean classic dataset from 
    - TensorFlow dataset https://www.tensorflow.org/datasets  
    - Sklearn toy datasets https://scikit-learn.org/stable/datasets/toy_dataset.html
- Load the dataset such that it is split between training and testing datasets 
- Design the supervised learning model of the neural network 
- Train the neural network so that it can correctly predict a continuous output variable or classes from the data set. 
- Overfit the neural network 
- Graph the model performance as it overfits the neural network 
    - How does the model score on the train data set (loss, accuracy) as it continues to train? 
    - How does the model score on the test dataset as it continues to train? 

### Search 
- Study and evaluate search algorithms based on four types of AI search: 
    - Uninformed search: depth-first search, breadth-first search, iterative deepening, etc. 
    - Informed search: Best first search, greedy search, A* 
    - Local search: hill climbing and its variants 
    - Adversarial search: mini-max, alpha-beta pruning, Monte Carlo tree search 
- Select appropriate problem(s) to be solved with the AI search algorithms you are studying 
- Find descriptions of AI algorithms that solve the problem you've selected 
    - Outline algorithm descriptions in your report 
- Find high-quality open-source AI search algorithm implementations that solve the chosen problems 
    - Include these implementations in your codebase. 
    - Modify, adjust, refactor, and document, as appropriate 
- Demonstrate and evaluate the algorithm's efficiency (time efficiency, space efficiency) on various problem inputs

### Fine-tuning a transformer
- Use Hugging Face pre-trained transformers (e.g., BigScience Large Open-science Open-access Multilingual Language Model - BLOOM, or AI2 OLMo adapted models), or other available transformers, as appropriate to your system. 

- Prepare the dataset 
    - Scrape data source into a plain text or CSV file (either manually or using automated scraping with BeautifulSoup, for example) 
        - Example of data source: academic integrity policy 
    - Separate content of text file into sequences (sentences) represented on separate lines (rows) to train the model on 
    - Transform the data set into a Python list or dataframe (either manually by creating the content of the data structure, or automatically using Python libraries) 
- Download the transformer and install the transformer model 
- Fine-tune and train the model on the selected dataset 
- Evaluate performance using question-answer format 
- Use WebUI https://github.com/oobabooga/text-generation-webui  

### Constraint programming (CP) 
- Decide the type of problem that the constraint solver will solve: 
    - Optimization problem, such as the assignment problem or scheduling problem 
    - Puzzles, such as cryptarithmetic puzzle, Sudoku, crossword puzzle, etc.  
- Find examples of constraint-based representations of the selected problem 
- Design and implement a constraint solver using two Google OR Tools constraint optimization solvers: 
    - CP-SAT solver 
    - CP traditional solver 
- Evaluate and compare performances of the two implementations.

###  Fine-tuning object detection 
- Find a suitable Kaggle dataset for the class you want to train on 
- Familiarize yourself with LabelMe (an open-source label annotation tool) http://labelme.csail.mit.edu/Release3.0/ and https://github.com/wkentaro/labelme  
- Install labelme and use it to create JSON labels 
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