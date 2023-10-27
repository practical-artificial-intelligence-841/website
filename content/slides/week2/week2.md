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

# Artificial Neurons​
Intro to Neural Networks​
COMP 741/841 Week 2​
Fall 2023​

## Agenda​
- Attendance (5 min)​
- Presentation (10-15 min)​
- Lab (50 min)​
    - Development tools​
        - git, conda, Python virtual environments, Jupyter Notebooks​
    - Minlab and MNIST lab​
        - CIFAR-10​
- History of ML and Artificial Neurons (30 min)​
- Due next week (10 min)​

## Presentation​
- Eric Lipton. 2023. A.I. Brings the Robot Wingman to Aerial Combat. New York Times. ​
- Rachel Thomas. 2023. AI and Power: The Ethical Challenges of Automation, Centralization, and Scale. fast.ai. [https://www.fast.ai/posts/2023-07-29-ai-centralizes-power/](https://www.fast.ai/posts/2023-07-29-ai-centralizes-power/)

Presenters​
- Priyanka and Paritosh(M2)
- David and Long(M1)
- Maneesh and Venkat(M4)
- Harsha and Deepthi(M3)

## Development Tools - Git​
- git versus GitHub​
    - git – version control system​
    - GitHub – Microsoft-owned service for storing and managing remote git repos​
- Cloning repos​
    - From GitHub org of the course: [https://github.com/2023-fall-comp-741-841/](https://github.com/2023-fall-comp-741-841/) ​

## Development Tools - Git​
- Committing​
    - git status​
    - git add file​
    - git status​
    - git commit –m ‘meaningful message starting with a VERB, e.g, add package X to …’​
    - git status​
- Collaboration
    - git checkout –b my-new-branch​
        - git push origin my-new-branch​
    - git checkout main​
 ​
## Development Tools – Python Virtual Environment​
- What is a virtual environment?​
    - Isolated Python environment – does not interact with global/user home directory​
    - Built-in support with Python 3 built-in module venv (part of Python standard lib)​
        - python –m venv my_env ​
        - Uses installed Python version (that’s on the $PATH and has alias python in case there are multiple installations) ​
- Why use virtual environments?​
    - To manage versions  and dependencies of packages by isolating them into the same environment​
    - To avoid installing packages globally (root directory) or user home directory​

## Development Tools – conda​
- **conda** - Package & virtual environment management system​
    - Used for Python and other programming languages, runs on Windows, MacOS, Linux​
    - Creates and manages virtual environments​
    - Verifies that current environment installations do not conflict with new installations​
    - Installs Python instances​
    - Bundled with Anaconda and Miniconda​

## Development Tools – conda​
- Anaconda platform - contains​
    - Distribution of Python and R​
    - Lots of packages automatically installed (~250) and more (~1,500)​
    - GUI, CLI, …, and **conda**​
- Miniconda – “bootstrap” version of Anaconda contains:​
    - Distribution of Python​
    - **conda**, and a small set of packages that **conda needs​**

## Development Tools – Jupyter Project​
Provides tools for **interactive computing** across many programming languages​

- Jupyter **kernel**​
    - Run-time environment for a specific programming language​
- **ipykernel** – provides IPython (Python kernel) for Jupyter​
- Jupyter Server​
    - Backend (core services and API) to a Jupyter application​
- JupyterHub​
    - Multi-user system​
    - Manages multiple instances of single-user Jupyter servers​

## Development Tools – Jupyter Project​
- Jupyter Stack – layered services for​
    - Users of Jupyter applications​
    - DevOps of Jupyter applications (deploy and serve Jupyter apps to others)​
    - Contributors to the Jupyter Server library​
- Jupyter notebook (formerly IPython notebook)​
    - Web application that creates and runs **interactive  computational documents​**
- Computational document (or notebook)​
    - Made of **cells** ​
    - Cells contains code, text (written in Markdown), visualizations, and more​

## Development Tools – Jupyter Project​
- Managed by a kernel (run-time environment)​
    - **ipykernel** runs selected Python-based notebooks (file extension **.ipynb**)​
    - Notebook cells can be run in any order​
    - Variables are saved and managed by the kernel​
- JupyterLab – newer user interface than the classic notebook​
    - Available in GitHub coding platform Codespace​
- Amazon SageMaker Studio Lab (SMSL)​
    - Web-based interactive development environment for notebooks, code ,and data​
    - Based on JupyterLab​
    ​
## Image Classification with MNIST​
- What is MNIST?​
    - Dataset of handwritten digits​
    - Occasionally considered the "Hello World" of machine learning
- What is image classification in context of AI?​
    - Neural network can identify and classify images it hasn't 'seen' before​
    - Neural network can't distinguish between multiple objects in image​
        - What happens if a model trained on MNIST is given an image with two digits?​
- What are some real-world use cases for image classification?​

## minilab and lab-mnist – Getting Started​
- Everyone will need to join the COMP841 GitHub organization​
    - 2023-fall-comp-741-841​
    - Home for labs, notebooks, scripts, and markdown
- Have either the instructor or the classroom assistant invite you using your GitHub username
- SageMaker Studio Lab (SMSL)​
    - See week2-sagemaker-studiolab-guidelines in the course OneDrive​
    - GitHub authentication: Personal Access Token, GitHub CLI (gh), or openssh​

## minilab and lab-mnist – Getting Started​
- minilab-stochastic-gradient-descent (minilab1)​
    - Get access to minilab1: [https://classroom.github.com/a/gza_N0_p](https://classroom.github.com/a/gza_N0_p) ​
    - Clone to SMSL and run it through the setup and lab instructions​
- lab-mnist
    - Get access to lab-mnist: [https://classroom.github.com/a/JZZx5_3f](https://classroom.github.com/a/JZZx5_3f)​
    - Clone to SMSL and follow lab instructions​

## ML Timeline and the Perceptron​
See resources in the course OneDrive​
- **week2-machine-learing-timeline**
- **week2-the-perceptron**

## Due Next Week​
- Assigned reading and reading notes​
    - Lefkowitz, Melanie. 2019. Professor’s perceptron paved the way for AI – 60 years too soon. Cornell Chronicle.  [https://news.cornell.edu/stories/2019/09/professors-perceptron-paved-way-ai-60-years-too-soon](https://news.cornell.edu/stories/2019/09/professors-perceptron-paved-way-ai-60-years-too-soon)
    - Tim Chalberg. 2009. Regression Analysis: A Powerful Tool and Riveting Drama. History of Mathematics Special Interest Group Mathematical Association of America (HOM SIGMAA) Student Paper Contest. [https://maa.org/sites/default/files/pdf/upload_library/46/HOMSIGMAA/Chalberg-RegressionHistoryPaper.pdf](https://maa.org/sites/default/files/pdf/upload_library/46/HOMSIGMAA/Chalberg-RegressionHistoryPaper.pdf)

## Due Next Week​
- Presentation​​
    - M1: Latha and Raunak
    - M2: Shiva and Sindhu​
    - M3: Anjali and Rashmi​
    - M4: Kalyan and Sai Venkat​
- Lab1: lab-mnist​
​