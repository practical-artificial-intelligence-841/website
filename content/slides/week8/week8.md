---
marp: true
draft: false
theme: uncover
headingDivider: 2
paginate: true
style: |
  section {
    text-align: left;
    font-size: 26px;
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

# Bias​
**Examples​**
### Discipline-specific Bias Concepts and Theories​
### Bias in Supervised Learning

COMP 741/841 Week 8​
Fall 2024

## Agenda

## Lab 5 Feedback and Discussion
- Solution is entirely based on the Google OR CP-SAT implementation illustrated in the n-queens example​
- Incremental development is more than multiple commits​
- A large number of commits can be as unhelpful as a single commit​
    - Where to look when something goes wrong? Now have to search through large commit history​
- Don't start incremental commits after completing the problem​
    - This is incremental commits, not incremental development​

## Lab 5 Feedback and Discussion
- Ex. of incremental development​
    - Commit requirements.txt​
    - Commit n-queens NQueenSolutionPrinter​
    - Clean and commit NQueenSolutionPrinter using pylint and pycodestyle​
- Docstrings should be descriptive​
    - "solves the problem with constraint programming" is not descriptive​
- n-queens main() performs the bulk of the work – this should be reflected​
    - What constraints are required? What variables are we using? What is the expected output?​

## Lab 5 Feedback and Discussion
- If docstring becomes too long, consider refactoring the function in several​
    - A long docstring could be a sign that the function is doing more than just one thing!​

To learn more about see applying CP-SAT to implement optimization problem solutions, see:​
- Champion, Antoine. 2020. When you can use constraint solvers instead of machine learning. Medium: Towards Data Science.  https://medium.com/towards-data-science/where-you-should-drop-deep-learning-in-favor-of-constraint-solvers-eaab9f11ef45 ​
- Labonne, Maxime. 2022.  Introduction to Constraint Programming in Python. GitHub.io ML Blog https://mlabonne.github.io/blog/. https://mlabonne.github.io/blog/posts/2022-05-02-Constraint_Programming.html  ​

## Reading Notes (RN8)
Denning, Peter J., and Dorothy E. Denning. 2020. Dilemmas of Artificial Intelligence. Communications of the ACM 63 (3): 22–24. https://doi.org/10.1145/3379920.​

