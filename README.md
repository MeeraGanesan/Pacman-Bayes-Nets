# Pacman-Bayes-Nets

Note: Code is kept private, can show on a need-to-know basis. Attributed to UC Berkeley (http://ai.berkeley.edu)

This project uses Bayes Nets to help Pacman eat all the ghosts (goal state). The agent has sensors that give the approximate distance between Pacman and a ghost.

When an observation (the noisy reading of the distance to the ghost) is made, the probability of the noisy distance reading given Pacman’s position and the ghost’s position is returned. The agent's belief distribution over ghost positions given an observation is then updated. However, since the ghost can move, a predicition is made at each time step to obtain a distribution over new positions for the ghost, given its previous position.

By using a simple greedy strategy, Pacman hunts the ghost by assuming it is in its most likely position according to Pacman's beliefs. 

This is extended to games where there are multiple ghosts.

