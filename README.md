# Email Network Analysis

## Introduction
- The Enron email communication network offers a case study for understanding complex organizational structures through the lens of social network analysis. 
- This project focuses on the detection of communities within the Enron email dataset, which encapsulates interactions among over a thirty-six thousand unique emails
- Dataset was originally disclosed by the Federal Energy Regulatory Commission during its investigation.

## Problem Statement
Identify communities in the email-Enron dataset.

## Data
[SNAP Stanford](https://snap.stanford.edu/data/email-Enron.html)
- Data is an undirected graph with 37K nodes and 183K+ edges.

## Community Detection Report
Click [here](https://github.com/k-lohani/email_network_analysis/blob/main/Network_Analysis_Report.pdf) for the report in pdf format

## Community Detection Algorithm Evaluation
Used modularity and conductance metrics along with visualization to narrow down the best performing algorithms.

## Steps
1. Preprocess the .txt file with the graph data.
2. Create edges using the Enron data.
3. Create Graphs using the edges created in step 2.
4. Data Proprocessing and Cleaning:
    - Removing Non-Enron Nodes using Statistical analysis
    - Component Analysis: Filtering small communities
    - Taking out the largest subsection for community detection
    - Removing Isolated Nodes
5. Graph EDA
6. Community Detection:
    - Louvain Algorithm
    - Label Propogation Algorithm
    - Lieden Algorithm
    - Infomap Algorithm
    - Walktrap Algorithm
    - Markov Clustering Algorithm
    - Girvan-Newman Algorithm (Level 7 to Level 20)

## Results
1. <strong>Best performing community detection model</strong><br> 
- Girvan-Newman Algorithm (Level 20 with 21 communities) with the modularity of 0.94 and conductance of 0.005. 
- Girvan-Newman was chosen the best instead of Louvain (modularity- 0.97) due to the conductance of Louvain (0.015) being higher
2. <strong>Worst performing community detection model</strong><br>
- Markov Clustering Algorithm (Communities - 633) with the modularity of 0.001 and conductance of 0.26.
