![Team Banner](/images/Team%20Banner.png)
# RoboCup SSL Software Team Recruitment Tasks 2025-26
Welcome to the recruitment process for the RoboCup SSL Software team! This repository contains two tasks designed to evaluate your understanding of computer vision, machine learning, and data processing in the context of robotic soccer.

## Task 1: Path Planning and Obstacle Navigation

### Overview
In this task, you will design and compare pathfinding algorithms that help a RoboSoccer robot navigate toward the ball while avoiding obstacles.

#### Create a Field Simulation
- Represent a RoboSoccer field as a **2D grid** (e.g., 20×20 or 30×30).  
- Mark positions for:  
  - **Robot (R)** → starting point  
  - **Ball (B)** → goal  
  - **Obstacles (O)** → walls or opponent robots  
- Randomize the placement of obstacles to generate multiple test cases.  

#### Implement and Compare Algorithms
Implement at least **two pathfinding algorithms**:
- **Breadth-First Search (BFS):** explores all possible paths to reach the goal.  
- **A\*** (or **Dijkstra’s Algorithm**): uses cost and heuristic values for efficient navigation.  

For each algorithm, measure and record:
- Total **path length**  
- **Execution time**  
- **Number of explored steps**  

Store your results in a simple **table or CSV file**.  

#### Visualize the Simulation
Use **Matplotlib** or **Pygame** to visualize your grid, showing:
- The robot’s movement path (colored line)  
- Obstacle positions  
- Ball location  

Optionally, animate the robot’s movement step by step.


#### Evaluate and Analyze Results
Run both algorithms on at least **three different grid configurations** with varying obstacle density.  
Compare their efficiency and explain **which algorithm performs better and why**.

#### Deliverables
- Code file (`.py` or `.ipynb`) containing both algorithms  
- Screenshot or visualization output of your pathfinding simulation  
- CSV or table comparing results (path length, time, steps)  
- Short explanation (~200 words) of your methodology and findings  

---



## Notes
- We prioritize methodology and clear understanding over complex analysis
- Focus on communicating your findings effectively
- Show your ability to extract meaningful insights from sports data
- You don't need to analyze the entire database - choose specific aspects that interest you
- Time management is important - complete the basic requirements before attempting optional tasks

Good luck with your submission! If you have any questions, please reach out through the appropriate channels.
