![Team Banner](/images/Team%20Banner.png)

# RoboCup SSL Software Team Recruitment Tasks 2026-27

## Welcome to the recruitment process for the RoboCup SSL Software team! This repository contains two tasks designed to evaluate your understanding of computer vision, machine learning, and data processing in the context of robotic soccer.

# Task 1: A-Star vs. BFS Pathfinding Mini-Challenge

## Overview

Your goal is to find the most efficient path for a robot on a grid to reach a ball, avoiding obstacles. You will implement and compare two classic algorithms, BFS and A\*, on a single, pre-defined field to see how they perform.

---

## Part 1: Setup & Algorithm Implementation

### 1.1 The Field

Instead of generating multiple fields, you will use this one 10x10 grid. Represent it as a 2D list or NumPy array.

Example:

```python
# 0=Empty, 1=Obstacle, 2=Robot, 3=Ball
grid = [
    [0, 0, 0, 0, 0, 0, 1, 0, 0, 0],
    [0, 2, 0, 1, 0, 0, 1, 3, 0, 0], # Robot at (1,1), Ball at (1,7)
    [0, 0, 0, 1, 0, 0, 1, 0, 0, 0],
    [0, 1, 1, 1, 0, 0, 0, 0, 0, 0],
    [0, 0, 0, 0, 0, 1, 0, 1, 0, 0],
    [0, 0, 1, 0, 0, 1, 0, 1, 0, 0],
    [0, 0, 1, 0, 0, 1, 0, 1, 0, 0],
    [0, 0, 1, 0, 0, 0, 0, 1, 0, 0],
    [0, 0, 0, 0, 1, 0, 0, 0, 0, 0],
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
]
start_pos = (1, 1)
goal_pos = (1, 7)
```

Create your own grid and use it.

---

### 1.2 Implement Algorithms

Implement two functions that take the grid, start, and goal positions as input. The robot can move Up, Down, Left, and Right.

1. **Breadth-First Search (BFS):**
   An algorithm that explores layer-by-layer. It's guaranteed to find the shortest path in terms of steps.

2. **A\* Search:**
   A "smarter" algorithm that uses a heuristic to guide its search.
   Use the Manhattan Distance for your heuristic:
   `h = |x1 - x2| + |y1 - y2|`

Each function should return two things:

- The final path (a list of coordinates)
- The number of nodes explored

---

## Part 2: Visualization & Evaluation

### 2.1 Visualize the Paths

Create two visualizations using matplotlib—one for the BFS result and one for the A\* result. Each plot should clearly show:

- The grid with obstacles
- The final path taken by the robot

---

### 2.2 Compare the Results

Run both algorithms on the grid and print the key results to the screen.

Example output:

```
BFS Algorithm:
Path Length: 12
Nodes Explored: 58

A* Algorithm:
Path Length: 12
Nodes Explored: 25
```

This direct comparison is enough to see the difference in efficiency.

---

### Deliverables

A single Jupyter Notebook (`.ipynb`) containing:

1. The code for your BFS and A\* implementations.
2. The two output visualizations (one for each algorithm's path).
3. The final printout of the path length and nodes explored for both algorithms.

---

## **Task 2: Transfermarkt Football Data Analysis & Valuation Modeling**

### **Overview**

Work with the **Transfermarkt Football Player Dataset** from Kaggle, which includes detailed player valuations, performance records, and updates.
Your goal is to **analyze**, **interpret**, and optionally **predict** player market values based on performance and attributes.

---

### **Part 1: Exploratory Data Analysis (EDA)**

Create at least **three visualizations** that provide meaningful insights into player performance, valuation, and financial trends across clubs and leagues.
Each visualization should include a short interpretation explaining the observed trend or relationship.

---

### **Part 2: (Optional) Simple ML Application**

Develop a basic **machine learning model** to predict **player market value** or **performance** using features such as age, position, height, and stats (goals, assists, minutes played).

---

### **Deliverables**

* A **Jupyter Notebook (.ipynb)** or **Kaggle/Colab link** containing:

  * Complete data analysis and visualizations
  * Interpretations and key findings
  * (Optional) Machine learning model and evaluation metrics
* At least **three labeled visualizations** with clear explanations
* A **short written summary** of your methodology, insights, and conclusions

---
## Resources

- **Dataset:** Football Data from Transfermarkt on Kaggle
- **Tools:** Kaggle Notebooks, Google Colab, or a local Jupyter environment
- **Python Libraries:** `pandas`, `matplotlib`, `seaborn`, `scikit-learn`

---

## Notes

- We prioritize methodology and clear understanding over complex analysis
- Focus on communicating your findings effectively
- Show your ability to extract meaningful insights from sports data
- You don't need to analyze the entire database - choose specific aspects that interest you
- Time management is important - complete the basic requirements before attempting optional tasks

Good luck with your submission! If you have any questions, please reach out through the appropriate channels.
