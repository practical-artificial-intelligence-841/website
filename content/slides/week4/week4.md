---
marp: true
draft: true
theme: uncover
headingDivider: 2
paginate: true
style: |
  section {
    text-align: left;
    font-size: 28px;
  }
  ul, ol, li {
    margin-left: 0;
  }
  h2 {
    font-size: 110%;
    color: #0000DD;
  }

_class:
 - lead
 - invert
---

# Neural Networks
COMP 741/841 Week 4​
Fall 2023


## Agenda

- Academic integrity (5 min)
- Presentations (15 min)
- Lab3: Sequential neural networks (50 min)
- More on machine learning, deep learning, and neural networks (15 min)
- Review
    - **week4-the-perceptron**
    - **Week4-neural-networks-basics**
- RN2 feedback (5 min)
- Due next week (5 min)

## Academic Integrity

#### If academic integrity misconduct continues, do you want to:

- Replace team project with a final exam?
- Replace presentations with 15-min quizzes on assigned readings?
- Replace labs with two exams?

#### What other changes IF our learning environment:

- Lacks trust
- Educational time is spent on checking authenticity instead of
    - Giving feedback to presentations, reading notes, and labs
    - Facilitating and guiding team projects

## Presentations

#### RN

- Henry Kautz. 2020. “The Third AI Summer.” Presented at the Association for the
    Advancement Artificial Intelligence Conference, New York, NY, USA, February 12.
    https://www.youtube.com/watch?v=_cQITY0SPiw. **_Only Part I: History of AI_**
- Kautz, Henry A. 2022. “The Third AI Summer: AAAI Robert S. Engelmore Memorial
    Lecture.” AI Magazine 43 (1): 105–25. https://doi.org/10.1002/aaai.12036. **_Only the_**
    **_first 6 sections (up to AI for Bad)._**

## Presentations

###### Presentation slides

- See **presentation-schedule.docx** in OneDrive to know how RN3 readings are divided
    among the presenters
- Presenters
    - M2: Shashank and Charishma
    - M1: Greeshmaand Lokesh
    - M4: Pavani and Saketh
    - M3: Jaya and Ashok

## Lab3: Sequential Neural Networks

- Revisits Keras sequential model
- Guided walk-through
- Fork **lab3-sequential-neural-networks** from the GitHub course org by accepting the GitHub classroom invitation shared in your section Discord channel
- Clone lab to your SageMaker CPU instance
- Create Markdown cells before each code cell detailing what the code is performing
    - Markdown cells _must_ be **_entirely_** in your own words

## Machine Learning vs Deep Learning

**Machine Learning**
* Subfield of AI
* Mathematical basis
    * Statistics (regression, decision trees)
    * Linear algebra (matrix computations)
    * Calculus (gradient descent)
* Idea: the machine "learns from data"
    * Uses large data sets (100 points/feature)
    * "Trains" on complex mathematical models
    * Finds correlations between known inputs and outputs
    * Predicts (automatically generates) outputs for unknown inputs
* Requires significant computing power

## Machine Learning vs Deep Learning

**Deep Learning**
* Subfield of ML
* Mathematical basis
    * Same mathematical basis
* Idea: the machine learns from data using neural networks
* Uses much larger data sets (thousands points/feature)
* Requires much more computing power

**Source:** AWS. 2023. What’s the difference between ML and DL.(https://aws.amazon.com/compare/the-difference-between-machine-learning-and-deep-learning/)

## Machine Learning vs Deep Learning

- ML: Subfield of AI
- Mathematical basis
    - ... see previous slide
- Idea: the machine “learns from data”
    - Requires **_feature engineering_**
       - human intervention to
          - Extract features, label data, assign weights
    - Suited for **_structured data_**
       - E.g. Predict customer’s cancel subscription based on their usage of the service
       - E.g. Recommend movies based on customer’s history of movie watching

## Machine Learning vs Deep Learning

- DL: Subfield of ML Wikipedia.
- Same mathematical basis as ML
- Idea: the machine learns from data using neural networks
- Removes or minimize need for humans
- Suited for **_unstructured data_**
    - Challenge: identify complex relationships
    - E.g. Predict user “sentiment” from social media data
    - E.g. Image classification, natural language processing

**_Source_** : AWS. 2023. What’s the difference between ML and DL. https://aws.amazon.com/compare/the-difference-between-machine-learning-and-deep-learning/

## Machine Learning vs Deep Learning*
##### Machine learning
- Training methods
    - Supervised
    - Unsupervised
    - Semi-supervised
    - Reinforcement
- Performance
    - Better on simpler tasks
    - E.g. Detect spam messages
- Human understanding
    - Sometimes easier
    - Depends on the mathematical model
       - E.g. decision trees
**_*Source_** : AWS. 2023. What’s the difference between ML and DL. https://aws.amazon.com/compare/the-difference-between-machine-learning-and-deep-learning/