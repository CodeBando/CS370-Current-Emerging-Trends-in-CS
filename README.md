# CS370-Current And Emerging Trends in Computer Science
This repository holds the final project from my Current and Emerging trend in Computer Science Course, and AI pathfinding system. Details regarding the application and project are below.

## Project Overview

### Project Description
The goal of this project was to design an intelligent agent for a treasure hunt game. The intelligent agent represents a pirate who's goal is to navigate a maze of pathways and obstacles to find a treasure before the player does. This project involved utilizing provided code and code developed by myself. 

### Provided Code:
The code provided to me included three files. Two Python files and a JuypterNotebook file. <br>
#### Python files
* TreasureMaze.py
<br>This is a Python class file that is utilized to define the enviroment, with a maze represented as a matrix. It also handles the state of the maze as the agent navigates it, providing rewards for each movement. It is also utilized to ensure the game will not go on indefinetly by defining a minimium reward, that if reached, will end the game. <br>

* GameExperience.py
<br> This is a Python class that is utized to store the episodes during training and to be utilized through training for explotation. As the model completes its training, it will pull from it's past learnings to ensure the highest possible reward. <br>

#### Jupyter Notebook File
* Bandyk_Matthew_ProjectTwoMilestone.ipynb
<br>The Jupyter Notebook file provided included the code to handle the creation of the enviorment utilizing the provided python code, a completed neural network, and code to test the agent after it has been trained. I was asked to complete the Q-Learning algorithm that would be utilized to train the neural network. <br>

## Project Review

### Overview of my work
The work I completed for this project included the development of a Q-Learning algorithm that was utilized to train the neural network and ensure the agent could navigate the maze to find the treasure. The completed algorithm functions as follows:
* Initialization: The agent starts at a random point in the maze.
* Exploration or Exploitation: At each step, the agent decides to either try a new path, which would be exploration, or follow a path it already knows, which is explotation. The algorithm was set to a 1:10 ratio of exploration to explotation.
* Action Taken: The agent completes it action, which provides it a reward which is stored.
* Learning: After each action, the agent remembers what it did, the reward it received, and where it ended up. It uses this information to update its understanding of the maze and improve its decision-making for the next steps.
* Training Neural Network: The neural network then learns from the experience as more and more actions are taken. It adjusts its strategy to maximize rewards, gradually getting better at navigating the maze.
* Evaluation: The agent repeats this over many epochs until it reaches convergance at which point the agent is trained to complete the maze.

## Question responses

### What do computer scientists do and why does it matter?
Computer scientists study algorithms, data structures, and systems to solve complex problems efficiently. They design and develop software, analyze and interpret data, and explore the theoretical foundations of computation. Their work matters because it drives technological innovation, powers advancements in various industries, and enables solutions to pressing global challenges.
<br>
### How do I approach a problem as a computer scientist?
As a computer scientist, I approach a problem systematically by first understanding its requirements and constraints. Then, I break down the problem into smaller, manageable parts, identify potential solutions, and evaluate their feasibility and efficiency. Collaboration, creativity, and critical thinking are essential in devising effective strategies and implementing robust solutions, leaning on peers to support and answer questions in the work I do.
<br>
### What are my ethical responsibilities to the end user and the organization?
As a computer scientists, I have ethical responsibilities to both end users and organizations. I must prioritize user privacy, security, and accessibility when designing and deploying software systems. Additionally, they should adhere to professional codes of conduct, ensure transparency in their decision-making processes, and actively mitigate the risks of bias, discrimination, and harm associated with technology and AI systems. Furthermore, I must promote a culture of integrity, accountability, and continuous improvement within my work to foster trust and sustainability.
<br>
