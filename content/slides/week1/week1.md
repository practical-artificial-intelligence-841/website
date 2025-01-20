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

# Welcome to COMP741/841 Practical Artificial Intelligence
### COMP 741/841 Week 1

## Agenda
- Introduction
- Course information
    - Syllabus, requirements, resources
    - Activities, schedule, assessment
    - Policies​
- Due next week
    - Tools: communication, reading,  writing, and development​
    - First assignment: research notes draft (RN1 Draft)​
- What is AI?

## Introductions
- What is your preferred given name? ​
- What do you like the most about computing?​
- What do you dislike the most about computing?​

Fill in the attendance sheet: first 5 minutes of each class​

## Course Information
- Weekly 2 hr 50 min class meetings: bring your laptop and charger!​
- Resources​
    - Canvas, GitHub, Zoom (if needed), Zotero​
    - Readings: ​
        - Wikipedia’s outline of AI: [https://en.wikipedia.org/wiki/Outline_of_artificial_intelligence](https://en.wikipedia.org/wiki/Outline_of_artificial_intelligence)
        - Wikipedia AI [https://en.wikipedia.org/wiki/Artificial_intelligence#](https://en.wikipedia.org/wiki/Artificial_intelligence#)
    - Zotero Practical AI group library: [https://www.zotero.org/](https://www.zotero.org/)​
        - See [Zotero Guidelines](https://practical-artificial-intelligence-841.github.io/website/resources-and-tools/zotero-intro/index.html) under **Resources and Tools** menu on left-hand side bar. 

## Course Resources: Development Tools​ and Services
Local tools
- Bash shell​
- Python 3
- Visual Studio Code
- git​
Cloud services
- AWS SageMaker Studio Lab
- Google Colab
- GitHub

## Learning Resources​
Course instructor, your peers​, CAE tutors, student tech consultants
- In-class and online Canvas participation​
- Study group sessions with peers and student tech consultants
- One-on-one check-ins with course instructor
- Tutoring in the Center for Academic Enrichment​

## Learning Activities, Assignments, and Assessment​
- 8 Research notes on assigned material, RNs (15%)​
    - Assigned every week, RN draft followed by RN final
    - Week 1 to Week 8
- 6 Lab projects (25%)
    - Assigned every week, Week 2 to Week 7
- Project Work (10%), starts Week 8
    - Proposal, Design, First Presentation
- Project Final (60%)​
    - Codebase, Report, Final Presenataion

## Learning Goals​
Balancing the **science of AI** with its **engineering applications**, you will learn:​
- The AI foundations and principles to build intelligent computational systems.
- How AI systems solve real-world problems that require:​
    - Reasoning, planning, learning, explaining, and acting with certainty and uncertainty ​
- The impact of AI on our society  and related ethical, privacy, security, and safety implications.  ​

## Competencies that the course helps you develop ​
- Explore and critique AI applications and their impacts
- Read and analyze relevant AI literature 
- Present, discuss, and evaluate AI approaches and technologies ​
- Examine, annotate, and evaluate sources of information  ​
- Develop a team project ​
- Cultivate professional qualities such as being responsible, persistent, adaptable, and self-reflective. ​


## What is Artificial Intelligence?​
As an academic discipline​
- Study of computational systems that act  intelligently (a.k.a. computational agents)​
- To act intelligently means​
    - Know what to do: Exhibit complex behavior to reach goals​
    - Know how to do it: ​
        - Sense, game play, reason, optimize, plan, process natural language, etc.​
    - Do it: Perform (or act) to meet those goals​
    - Learn: from past experience and prior knowledge​

## What is Artificial Intelligence?​
As a technology ​
- Software and tools platforms, services made by humans and used by humans​
As a professional career​
- Research scientist​
- Software developer/engineer​
- UX (user experience) designer​
- Data scientist, data engineer​
- More ...​

## Goals of AI​
- Scientific goal​
    - Understand how artificial and natural systems can act intelligently​
        - Analyze artificial and natural agents​
        - Formulate and test hypotheses about how to construct intelligent agents (AI)​
        - Design, build, experiment with computational systems that perform tasks that require intelligence​
- Engineering goal​
    - Design and make intelligent computational systems that are useful​
- Ethical goal

## Ethical Implications of AI and the Alignment Problem
**How to make AI align complex, autonomous systems with human norms and values?​**

AI systems as **objects** and their implications​
- Automation and unemployment​
- Privacy and manipulation​
- Human-robot interaction and autonomy​

AI systems as **subjects​**
- Machine ethics: ethics of AI systems themselves​
- Artificial moral agency​


## Ethical Implications of AI and the Alignment Problem
AI as **superintelligence​**
- singularity​

**Sources** ​
Brian Christian, The Alignment Problem, 2020​
Ethics of AI and Robotics, 2020, Stanford Encyclopedia of Philosophy, [https://plato.stanford.edu/entries/ethics-ai/​](https://plato.stanford.edu/entries/ethics-ai/​)


## Open and Closed Source Neural AI
What makes a neural AI system open or closed source?​
- Model weights are publicly available​
    - Model weights auditability versus classical programs​
    - What parameters were used to train the model?​
        - Can the results be replicated?​
- Dataset is publicly available
    - Is the dataset documented?​
        - Are limitations and biases explicitly defined?​
- AI-as-a-service​
    - ChatGPT, Bing AI, GitHub CoPilot​
        - CoPilot is trained on GitHub repos​
        - Would this be considered a publicly available dataset?​

## Human-Machine Teaming​
- AI as an assistant​
    - ChatGPT as a replacement for Google searches​
    - Article summarization​
- Human as the controller​
    - Human has final say as user – AI augments capabilities​
- Consequential versus non-consequential AI​
    - Shopping recommendations versus military use​
    - Human user has more control as potential consequences increase​
- Building trust in AI​
    - AI must produce accurate outputs, but also​
    - Reliable, safe, transparent, and explainable decisions​
​