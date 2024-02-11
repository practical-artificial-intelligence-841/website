---
title: Conda Basics
weight: 1
---
Quiz your understanding of the basic `conda`commands.

- What `conda` Python environment is activated and what do you know about it?
    - Answer: `conda info`
- What are the locations of all `conda` environments you currently have locally, on your 
laptop or in the cloud, for example in  your SageMaker Studio Lab account?
    - Answer: `conda env list`
- How can you deactivate the currently activated environment? 
    - Answer: `conda deactivate`
- How can you activate an existing environment, for example the **studiolab** environment?
    - Answer: `conda activate studiolab`
- How can you create a new virtual environment named `my-special-env`? 
    - Answer: `conda create --name my-special-env`
- How can you create a virtual environment, called `my-special-env` from a `.yml` file 
called `special_requirements.yml`?
    - Answer: 
    ```
    conda env create --name my-special-env --file='special_requirements.yml'
    ```
- How can you find out what packages are installed in the activated environment?
    - Answer: `pip list`
- How do you deactivate the current `conda` environment?
    - Answer: `conda deactivate`