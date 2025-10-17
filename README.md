# Community Detection in Social Networks using Graph Algorithms

## Overview

This project focuses on identifying **communities within complex networks** using advanced **graph-based algorithms**.  
It applies the **Girvan–Newman**, **Louvain**, and **Greedy Modularity** methods to detect and visualize clusters within network data.

The main objective is to demonstrate how **modularity optimization** and **edge betweenness** can reveal hidden relationships and subgroups in a graph structure, forming the foundation of modern social network analysis.

---

## Table of Contents
- [Concept](#concept)
- [Methodology](#methodology)
- [Results](#results)
- [Technologies Used](#technologies-used)
- [Usage](#usage)

---

## Concept

**Community Detection** is the process of discovering groups (or clusters) in which nodes are more densely connected to each other than to nodes in other groups.  
It plays a vital role in **social network analysis**, **recommendation systems**, and **biological network discovery**.

This project implements and compares three algorithms:
1. **Girvan–Newman Algorithm** – Uses edge betweenness to iteratively remove the most “central” edges.  
2. **Louvain Algorithm** – Maximizes modularity through hierarchical clustering.  
3. **Greedy Modularity Maximization** – Builds communities iteratively to improve modularity score.

---

## Methodology

1. **Graph Construction**
   - Imported dataset and converted it into a network using NetworkX.
   - Represented relationships as edges and individuals as nodes.

2. **Girvan–Newman Algorithm**
   - Computed edge betweenness centrality.  
   - Removed high-centrality edges iteratively.  
   - Extracted resulting communities.

3. **Louvain and Greedy Algorithms**
   - Applied Louvain and Greedy modularity approaches to compare performance and modularity.  
   - Measured **modularity score**, **number of communities**, and **community size distribution**.

4. **Visualization**
   - Used Matplotlib to display communities with unique colors and labels.

---

## Results

- **Girvan–Newman Algorithm** detected distinct community structures with clear modular boundaries.  
- **Louvain method** achieved the **highest modularity (~0.73)** and most balanced partitioning.  
- **Greedy modularity** produced faster results but with slightly lower modularity (~0.69).  
- Visualizations confirmed well-separated node clusters.  

*(All graphs and visualizations are displayed directly in the notebook.)*

---

## Technologies Used

- **Language:** Python 3.9+  
- **Libraries:**
  - NetworkX
  - Matplotlib
  - Community (python-louvain)
  - NumPy / Pandas
- **Tool:** Jupyter Notebook

---

## Usage

1. Clone this repository:
   ```bash
   git clone https://github.com/mehmet-akif/community-detection-graph-algorithms.git
   cd community-detection-graph-algorithms
   ```

2. Install dependencies:
   ```bash
   pip install networkx matplotlib community numpy pandas
   ```

3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook LAB11-AKIF-SIPAHI.ipynb
   ```

4. Run all cells to:
   - Generate and visualize a sample network  
   - Apply Girvan–Newman, Louvain, and Greedy modularity algorithms  
   - Compare modularity and community structure

---



## License

© 2025 Mehmet Akif Sipahi. All rights reserved.  
This project is shared for educational and portfolio demonstration purposes only.  
Reproduction, redistribution, or submission of this material for academic credit is strictly prohibited.
