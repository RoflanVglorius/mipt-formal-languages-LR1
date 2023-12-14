# mipt-formal-languages-LR1

Class ```State``` - state of the type ```A -> .aB```.  
Class ```Grammar``` - grammar.  
Class ```Automaton``` - deterministic finite automaton.  
  
   ```Automaton``` class fields:
1) ```nodes``` - nodes of the automaton.  
2) ```grammar``` - grammar.
3) ```processed``` - set of processed nodes while building the automaton.
4) ```built``` - set of processed states while building the table.
5) ```lr_table``` - table of transitions.
6) ```node_to_number``` - mapping from a node to its number.
7) ```number_to_node``` - mapping from a number to node.
8) ```start_node``` - starting node.
9) ```term_node``` - terminal node.
  
    
    
```Automaton``` class methods:
1) ```Build``` - runs automaton build.
2) ```ProcessNode``` - evaluates ```States``` in the node and adds edges.
3) ```EnumerateNodes``` - enumerates nodes.  
4) ```ProcessClosestTerminals``` - returns all closest terminal nodes from the derivation tree.
5) ```BuildTable``` - builds the table.
