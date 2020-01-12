![Supported Python Versions](https://img.shields.io/badge/Python->=3.6-blue.svg?logo=python&logoColor=white)

# Fire Forest - Celllular Automaton

*DECOURT Colin*

> This repository contain a school project simulating cellular automatons on a fire forest. This was done as part of the course *Intelligence distribuée* given by Laurent Simon at Bordeaux INP - ENSEIRB MATMECA. 

The code can be execute by download the repository and run the following Jupyter Notebook : [fire-forest.ipynb] [source]() |


## Description

All the code is in a Jupyter Notebook named : `fire-forest.ipynb`. This notebook is divided in several sections : 

  - ▶️️ Utils functions : contain functions for getting valid cells' coordinates and the neighbour cells coordinates
  - ▶️️ Parameters : parameters of the simulation and function for generating a forest with different tree densities and some clearing. 
  - ▶️️ Transition functions : contain state transition functions. Transition rules are :
      * An empty cell remain an empty cell
      * A ash cell stay ash
      * A fire cell become ash
      * A tree cell :
          * Become fire if one of them neighbour is in fire depending on the density (percolation threshold). The more the percolation threshold is high the more the tree will burn. 
          * Remain a tree otherwise
   - ▶️️ A step function which one propagation step. Get the actual state and output a new state depending on transition rules. 
   - ▶️️ Main cell : initialization of the forest, launch fire forest with different grid sizes until there is no more burning tree.
   - ▶️️ Data analyse : some plots to see impact of percolation threshold...

