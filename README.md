# Droplet
Droplet is a microRTS bot based on script guided MCTS. 

1. The base MCTS algorithm is called [Naive Sampling (NS) and NaiveMCTS](https://arxiv.org/abs/1710.04805), which is a variation of MCTS that designed to tackle the combinatorial multi-armed bandit problem. 

2. The main algorithm used in Droplet is Guided Naive Sampling (GNS), which uses one or more scripts to bias NS towards more promising space of the search.

3. The abstract actions in this repo (*Attack*, *Build*, *Harvest*, *Move*, etc.) are modified from the original ones from the microRTS repo such that the direction parameter is ramdomized instead of in a certain order. The modification can avoid some situation like when two units have conflicting paths.
