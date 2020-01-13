![Supported Python Versions](https://img.shields.io/badge/Python->=3.6-blue.svg?logo=python&logoColor=white)

# Fire Forest - Celllular Automaton

*DECOURT Colin*

> This repository contain a school project simulating cellular automatons on a fire forest. This was done as part of the course *Intelligence distribuée* given by Laurent Simon at Bordeaux INP - ENSEIRB MATMECA. 


The code can be execute by download the repository and run the following Jupyter Notebook : [fire-forest.ipynb](https://github.com/colindecourt/FireForest-CelllularAutomaton/blob/master/fire-forest.ipynb) 


## Description

There is two Jupyter Notebooks. 

### First Jupyter Notebook 

The second notebook called [percolation-fire-forest.ipynb](https://github.com/colindecourt/FireForest-CelllularAutomaton/blob/master/percolation-fire-forest.ipynb) is a cellular automaton where a map with different density of trees is generated (from 0% of tree to 95% of tree). This notebook is divided in several sections : 

  - ▶️️ Utils functions : contain functions for getting valid cells' coordinates and the neighbour cells coordinates
  - ▶️️ Parameters : parameters of the simulation and function for generating a forest with different density of trees (percolation threshold). 
  - ▶️️ Transition functions : contain state transition functions. Transition rules are :
      * An empty cell remain an empty cell
      * A ash cell stay ash
      * A fire cell become ash
      * A tree cell :
          * Become fire if one of them neighbour is in fire. The **Moor neighbourhood** was used. 
          * Remain a tree otherwise
   - ▶️️ A step function which one propagation step. Get the actual state and output a new state depending on transition rules. 
   - ▶️️ Main cell : initialization of the forest, launch fire forest with different grid sizes until there is no more burning tree.
   - ▶️️ Data analyse : some plots to see impact of percolation threshold...

   

##### Tree type burning simulation 


##### Impact of percolation threshold




### Second Jupyter Notebook 


The second notebook called [tree-density-fire-forest.ipynb](https://github.com/colindecourt/FireForest-CelllularAutomaton/blob/master/tree-density-fire-forest.ipynb) is a cellular automaton where a map with different tree type is generated. A tree will burn depending on the density (size for instance) of the tree. This notebook is divided in several sections : 

  - ▶️️ Utils functions : contain functions for getting valid cells' coordinates and the neighbour cells coordinates
  - ▶️️ Parameters : parameters of the simulation and function for generating a forest with different tree densities (four tree types) and some clearing. 
  - ▶️️ Transition functions : contain state transition functions. Transition rules are :
      * An empty cell remain an empty cell
      * A ash cell stay ash
      * A fire cell become ash
      * A tree cell :
          * Become fire if one of them neighbour is in fire depending on the density (the type of the tree). The more the density is high the more the tree will burn (non intuitive I know...). The **Moor neighbourhood** was used. 
          * Remain a tree otherwise
   - ▶️️ A step function which one propagation step. Get the actual state and output a new state depending on transition rules. 
   - ▶️️ Main cell : initialization of the forest, launch fire forest with different grid sizes until there is no more burning tree.
   - ▶️️ Data analyse : some plots to see impact of probability of burning...
   - ▶️️ **Pray for Australia** section : this is the same simulation but adapted to Australia forest map. Each type of forest have a density and will burn depending on it. 
   

##### Tree type burning simulation 

![Tree type - 50x50 grid](https://github.com/colindecourt/FireForest-CelllularAutomaton/blob/master/gif/(40%2C%2040)Gif-2020-23-12-21-23-36.gif)

##### Some plots...


##### Australia burning simulation...


