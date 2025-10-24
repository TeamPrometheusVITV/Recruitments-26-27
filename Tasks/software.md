![Team Banner](/images/Team%20Banner.png)
# RoboCup SSL Software Team Recruitment Tasks 2026-27
Welcome to the recruitment process for the RoboCup SSL Software team! This repository contains two tasks designed to evaluate your understanding of computer vision, machine learning, and data processing in the context of robotic soccer.
---

# Task 1: A-Star vs. BFS Pathfinding Mini-Challenge

## Overview

Your goal is to find the most efficient path for a robot on a grid to reach a ball, avoiding obstacles. You will implement and compare two classic algorithms, BFS and A*, on a single, pre-defined field to see how they perform.

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

2. **A* Search:**
   A "smarter" algorithm that uses a heuristic to guide its search.
   Use the Manhattan Distance for your heuristic:
   `h = |x1 - x2| + |y1 - y2|`

Each function should return two things:

* The final path (a list of coordinates)
* The number of nodes explored

---

## Part 2: Visualization & Evaluation

### 2.1 Visualize the Paths

Create two visualizations using matplotlib—one for the BFS result and one for the A* result. Each plot should clearly show:

* The grid with obstacles
* The final path taken by the robot

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

1. The code for your BFS and A* implementations.
2. The two output visualizations (one for each algorithm's path).
3. The final printout of the path length and nodes explored for both algorithms.

---

# Task 2: Transfermarkt Football Data Analysis & Valuation Modeling

## Overview

In this task, you will work with the comprehensive Football Player dataset from Transfermarkt, available on Kaggle. This dataset is unique for its detailed player market valuations, extensive appearance records, and regular updates. Your goal is to explore the data, uncover insights into player performance and valuation, and optionally build a machine learning model to predict player market values.

Dataset: Football Data from Transfermarkt

---

## Part 1: Basic Data Exploration

* **Load and Structure:**
  Load the multiple CSV files (`players.csv`, `clubs.csv`, `games.csv`, `player_valuations.csv`, `appearances.csv`, etc.). Explore the relationships between the files using their common IDs (e.g., `player_id`, `game_id`).

* **Data Quality Check:**
  Investigate the data for quality issues. Pay close attention to missing values in crucial columns like `market_value_in_eur` and performance stats like goals. Check for any duplicate entries.

* **Descriptive Statistics:**
  Provide summary statistics for key numerical variables, such as player age, height, market value, goals, assists, and minutes played.

---

## Part 2: Exploratory Data Analysis (EDA)

Create at least 3 visualizations that provide meaningful insights into the world of football finance and performance. Your analysis should be accompanied by a brief interpretation of each chart.

### Suggested Topics

**Market Value Analysis**

* Analyze the distribution of player market values across different leagues or positions.
* Investigate the relationship between a player's age and their market value. At what age does a player's value typically peak?

**Performance vs. Value**

* Is there a strong correlation between a player's market value and their performance metrics (e.g., goals, assists per 90 minutes)?
* Identify "undervalued" or "overvalued" players by comparing their performance statistics against their market value.

**Club & League Financial Power**

* Calculate and visualize the total market value of squads for different clubs or entire leagues. How does this financial power correlate with league standings?

**Nationality and Value**

* Which nationalities command the highest average market value? Create a bar chart or map to visualize this.

---

## Part 3: Simple ML Application (Optional)

Develop a basic machine learning model to address one of the following challenges.

### Suggested ML Tasks

**Player Market Value Prediction (Regression):**

* Build a model to predict a player's market value based on their attributes (age, position, height, foot) and recent performance statistics (goals, assists, minutes played).
* This is the primary recommended task for this dataset.

**Player Performance Prediction (Regression/Classification):**

* Predict the number of goals a forward will score in the next season based on their historical data.

**Identifying Player Potential (Classification):**

* Build a model to classify young players as having "high potential" (e.g., likely to see a significant market value increase) based on their early career stats.

---

## Deliverables

* A Jupyter Notebook (`.ipynb`) or a link to a Kaggle/Colab notebook containing your complete analysis, from data loading to final conclusions.
* At least 3 well-labeled visualizations with clear interpretations explaining what insights they reveal.
* A brief written summary of your methodology, key findings from the EDA, and overall conclusions.

If attempting the ML part:

* **Feature Selection:** Justify why you chose certain features for your model.
* **Model Choice:** Briefly explain your choice of algorithm (e.g., Linear Regression, Random Forest, Gradient Boosting).
* **Performance Metrics:** Report basic performance metrics for your model (e.g., Mean Absolute Error (MAE) or R-squared for regression; Accuracy or F1-score for classification).

---

## Resources

* **Dataset:** Football Data from Transfermarkt on Kaggle
* **Tools:** Kaggle Notebooks, Google Colab, or a local Jupyter environment
* **Python Libraries:** `pandas`, `matplotlib`, `seaborn`, `scikit-learn`

---

## Notes
- We prioritize methodology and clear understanding over complex analysis
- Focus on communicating your findings effectively
- Show your ability to extract meaningful insights from sports data
- You don't need to analyze the entire database - choose specific aspects that interest you
- Time management is important - complete the basic requirements before attempting optional tasks

Good luck with your submission! If you have any questions, please reach out through the appropriate channels.
