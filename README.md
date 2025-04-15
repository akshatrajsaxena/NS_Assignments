# Network Science Assignments

This repository contains the implementation of various network science concepts as part of a course on complex networks. The assignments explore fundamental algorithms, models, and analysis techniques used in network science.

## Overview

The repository includes three assignments (A1, A2, A3) that progressively build upon network science concepts:

1. **Assignment 1**: Basic network analysis and visualization
2. **Assignment 2**: Network models and robustness analysis
3. **Assignment 3**: Random graph models and network motifs

## Assignment 1: Network Representation and Basic Metrics

### Implementations:
- Network representation using adjacency matrices and edge lists
- Network visualization and export as image files
- Computation of fundamental network properties:
  - Network sparseness
  - Average degree ⟨k⟩
  - Degree distribution plotting (scaled/normalized)
  - Average path length using Breadth-First Search (BFS)
  - Average clustering coefficient
- Directed graph analysis:
  - In-degree and out-degree computation
  - In/out degree distribution plotting
- Weighted network analysis:
  - Weighted degree and clustering coefficient implementation
  - Distribution plotting for weighted networks
- Gilbert random graph generation and comparison with real-world networks
- Network visualization using Cytoscape with various layouts

## Assignment 2: Network Models and Robustness

### Implementations:
- **Watts-Strogatz Small-World Network Model**:
  - Implementation of the model with rewiring probability parameter
  - Analysis of scaled clustering coefficient and characteristic path length
  
- **Barabási-Albert (BA) Scale-Free Network Model**:
  - Implementation of preferential attachment algorithm
  - Parameter variations (initial network size, nodes/edges added at each step)
  - Network topology analysis (clustering coefficient, path length, degree distribution)
  
- **Modified Barabási-Albert Model**:
  - Implementation of a "super-rich-get-richer" model (attachment probability ∝ degree²)
  - Higher-order variants creation and analysis
  - Comparative study with standard BA model
  
- **Network Robustness Analysis**:
  - Random node deletion strategy
  - Impact measurement on characteristic path length
  - Giant cluster size measurement
  - Comparative robustness study between random and scale-free networks
  - Analysis of real-world scale-free networks under different attack strategies
  
- **Yeast Protein Interactome (YPI) Analysis**:
  - Construction from Yeast Interactome Database
  - Degree distribution and C(k) × k plotting
  - Network visualization using Cytoscape
  - Identification of essential proteins based on degree
  - Robustness analysis under random and targeted node deletion

## Assignment 3: Random Graph Models and Network Motifs

### Implementations:
- **Random Graph Models**:
  - Configuration Model implementation
  - Edge-Swapping strategy for random graph generation
  - Degree sequence preservation from real-world networks
  - Comparative analysis of degree distributions

- **Degree Correlation Analysis**:
  - knn vs k plots for real-world networks
  - Comparison with random graph counterparts

- **Network Motif Analysis**:
  - Implementation of algorithm to generate all unique 3-node connected subgraphs in directed networks
  - Z-score computation for subgraph significance
  - Identification of network motifs and anti-motifs

## Libraries Used
- NetworkX/igraph for network analysis
- Matplotlib/Seaborn for visualization
- NumPy/SciPy for numerical computations
- Cytoscape for advanced network visualization

## Data Sources
- Real-world networks with > 1000 nodes
- Yeast Protein Interactome from the Yeast Interactome Database (http://interactome.dfci.harvard.edu/S_cerevisiae/)
- Essential gene information from public data sources

## Requirements
- Python 3.x
- NetworkX/igraph
- Matplotlib
- NumPy
- Cytoscape (for visualization tasks)

## Usage
Each assignment folder contains Jupyter notebooks and Python scripts demonstrating the implementations. To run the code:

```bash
# Clone the repository
git clone https://github.com/akshatrajsaxena/NS_Assignments.git
cd network-science-assignments

# Install requirements
pip install -r requirements.txt

# Navigate to specific assignment
cd A1  # or A2, A3

# Run Jupyter notebooks
jupyter notebook
```

## Results
The repository includes visualization outputs and analysis results for each implementation, allowing for comparison with theoretical expectations from network science novelty.
