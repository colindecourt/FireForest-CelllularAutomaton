# Fire Forest - Celllular Automaton

This is a school project simulating cellular automatons on a fire forest.


## Description

All the code is in a Jupyter Notebook named : `fire-forest.ipynb`. This notebook is divided in several sections : 

  1. Utils functions : contain functions for getting valid cells' coordinates and the neighbour cells coordinates
  2. Parameters : parameters of the simulation and function for generating a forest with different tree densities and some clearing. 
  3. Transition functions : contain state transition functions. Transition rules are :
      * An empty cell remain an empty cell
      * A ash cell stay ash
      * A fire cell become ash
      * A tree cell :
          * Become fire if one of them neighbour is in fire depending on the density (percolation threshold). The more the percolation threshold is high the more the tree will burn. 
          * Remain a tree otherwise
   4. A step function which one propagation step. Get the actual state and output a new state depending on transition rules. 
   5. Main cell : initialization of the forest, launch fire forest with different grid sizes until there is no more burning tree.
   6. Data analyse : some plots to see impact of percolation threshold...
