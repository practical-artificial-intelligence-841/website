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

# Symbolic AI​
Search and Optimization​
COMP 741/841 Week 3​
Fall 2023​

## Agenda​
- Presentation (15 min)​
- Academic Integrity (20 min)​
- Symbolic AI: heuristic search (45-50 min)​
- Image classification (15-20 min)​
- Due next week (10 min)

## Presentation​
- Lefkowitz, Melanie. 2019. Professor’s perceptron paved the way for AI – 60 years too soon. Cornell Chronicle. ​
- Tim Chalberg. 2009. Regression Analysis: A Powerful Tool and Riveting Drama. History of Mathematics Special Interest Group Mathematical Association of America (HOM SIGMAA) Student Paper Contest. ​

Presenters
- Sindhu and Shiva (M2)​
- Latha and Raunak (M1)​
- Kalyan and Sai Venkat (M4)​
- Anjali and Rashmi (M3)

## Academic Integrity​
- RN1​
- RN1 Reflection​
- RN2 extended deadline​
- RN3

## Symbolic AI​
- AI paradigm, born in mid-1950s, went through “summers” and “winters”
- Collection of theories, techniques​
    - Inspired by how humans reason​
    - Based on symbolic representations of the problem, with entities that ​have meanings for humans​


## Examples of symbolic AI approaches and systems​
- Combinatorial (heuristic) search​
- Logic-based problem solvers, mathematical reasoning, automatic theorem proving​
- Game playing​
    - mini-max algorithm, alpha-beta pruning​
- Knowledge-based systems​
    - Expert systems, e.g., IBM’s Deep Blue (encoded chess expert knowledge, used alpha-beta search, and VLSI chips to parallelize the algorithm)​
- Probabilistic reasoning​
    - E.g., Hidden Markov Models (speech recognition)​
- Planning, Natural Language Processing (NLP), Satisfiability, Constraint Satisfaction, …​

## Symbolic AI vs Machine Learning​
- Symbolic – inspired by how humans reason​
    - Explainable​
        - Humans can follow how input changes through the algorithm into the output​
        - On different executions, same output is obtained for the same input​
    - Can be entirely algorithmic – no need for outside data​
    - Limited by​
        - Knowledge acquisition: domain knowledge experts are needed to represent the knowledge​
        - Rules of representation drive the reasoning: if a graph is required, a graph must be inputted​

## Symbolic AI vs Machine Learning​
- Machine Learning - inspired by how the brain functions​
    - Non-explainable, opaque​
        - Input to output can be traced, but the trace is unintelligible​
    - Requires large amounts of data​
        - MNIST (a simple task for today's standards) requires 60,000 train images​
    - Can 'learn' unintended routines​

## Lab 2: A* Search Algorithm ​
(a.k.a informed search  or best-first search algorithm​)
Solves the following **problem**:​
- Find the most cost-effective path from a specified **source** to a specified **goal​**

Problem **input representation: weighted graph** (nodes and edges)​
Problem **output representation**:
- A path in the graph, from source to goal, having the smallest cost (sum of the weights)​

Uses a **heuristic function h(n)**:
- The function calculates an estimate of the cheapest path from a node **n** to the **goal**

## Lab 2: A* Search Algorithm
- If **h(n)** is **admissible**, that is, it **never overestimates** the **actual cost** to get to the **goal​​**
- Then A* guarantees optimality, that is finds the **least-cost path** from **source** to **goal**

Applications​
- Find the shortest route on a map, **h(n)** can be the straight-line distance to the goal​
- Find the shortest route on a **grid map, h(n)** can be the **Manhattan distance**​

Algorithm idea ​
- Maintain a tree of paths that start at the **source** node​
- Extend those paths one edge at a time until ​
    - **goal** node is reached OR there is no eligible path to extend​


## Lab 2: A* Search Algorithm
At each iteration, determine which of the paths to extend with the **next node n** by calculating​
- **g(n)**: The cost of the path from the **source** to **next node n**  and​
- **Heuristic function h(n)**, which​
    - Estimates the cost of the **cheapest path** from **n** to the **goal**
- Such that **f(n) = g(n) + h(n)** is minimized​​

- Pseudocode: [https://en.wikipedia.org/wiki/A*_search_algorithm#Pseudocode](https://en.wikipedia.org/wiki/A*_search_algorithm#Pseudocode)
- Examples with animation: [https://en.wikipedia.org/wiki/A*_search_algorithm#Example](https://en.wikipedia.org/wiki/A*_search_algorithm#Example)

## Lab 2: A* Search Algorithm
- Implementation with explanations: ​
    - Andreas Soularidis: An Introduction to A* Algorithm in Python
    [https://medium.com/p/79475244b06f](https://medium.com/p/79475244b06f)
    - Also published on PlainEnglish at [https://plainenglish.io/blog/a-algorithm-in-python](https://plainenglish.io/blog/a-algorithm-in-python)

- GitHub URL from Andreas Soularidis public repo **medium_articles** [https://github.com/AndreasSoularidis/medium_articles.git](https://github.com/AndreasSoularidis/medium_articles.git)
    - See **AStarAlgorithm** folder​

## Lab2 Requirements​
- Create **comp841** directory in your home directory on your laptop​
    - Create **labs** subdirectory in **comp841**
- Fork **lab2** from the GitHub course org by accepting the GitHub classroom invitation shared in your section Discord channel​
- Clone lab2-xxx remote repo to your **labs** directory under the name **lab2​**
    - **git clone <remote-url>  lab2​**
- Launch PyCharm and open **comp841** directory. ​
    - In PyCharm **terminal**, select **git-bash** or **Ubuntu** shell​
    - Create **.venv** virtual environment in **comp841** and, in the **terminal**, check it is activated​
        - **which python**     - Should show path for Python instance in .venv directory​

## Lab2 Requirements​
- Install **pylint** and **pycodestyle** (pip install pylint and pip install pycodestyle)​
- Move to **lab2** and **mark directory as source root**. Run **main.py​**
- Examine the list of styling and coding errors reported in the **Problems** tab ​
- Create STYLE-LOG.md file to record types of errors you have fixed (touch STYLE-LOG.md)
- Run **pylint** and **pycodestyle** on all 3 Python files: main.py, a_star.py, graph.py​
- Fix as many errors as you can​
- Updated STYLE-LOG.md with new types of errors you’ve fixed.​
- Add in STYLE-LOG.md the types of errors you couldn’t fix. ​

## Due Next Week​
**Friday, Sep 15**: RN2​
**Monday, Sep 18​**
- Lab1​
- Lab2​
- RN3​
    - Henry Kautz. 2020. “The Third AI Summer.” Presented at the Association for the Advancement Artificial Intelligence Conference, New York, NY, USA, February 12. [https://www.youtube.com/watch?v=_cQITY0SPiw](https://www.youtube.com/watch?v=_cQITY0SPiw). **Only Part I: History of AI​**

    - Kautz, Henry A. 2022. “The Third AI Summer: AAAI Robert S. Engelmore Memorial Lecture.” AI Magazine 43 (1): 105–25. [https://doi.org/10.1002/aaai.12036](https://doi.org/10.1002/aaai.12036). **Only the first 6 sections (up to AI for Bad)**.​

## Due Next Week​
- Presentation slides​
    - See **presentation-schedule.docx** in OneDrive to know how RN3 readings are divided among the presenters​
    - Presenters​
        - M2: Shashank and Charishma​
        - M1: Greeshma and Lokesh​
        - M4: Pavani and Saketh​
        - M3: Jaya and Ashok​

