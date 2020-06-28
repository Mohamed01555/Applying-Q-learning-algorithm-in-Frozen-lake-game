# Applying-Q-learning-algorithm-in-Frozen-lake-game
* Frozen Lake description

-I’ve grabbed the description of the game directly from Gym’s website. Let’s read through it together.

Winter is here. You and your friends were tossing around a frisbee at the park when you made a wild throw that left the frisbee out in the middle of the lake.
The water is mostly frozen, but there are a few holes where the ice has melted.
If you step into one of those holes, you'll fall into the freezing water.
At this time, there's an international frisbee shortage, so it's absolutely imperative that you navigate across the lake and retrieve the disc
However, the ice is slippery, so you won't always move in the direction you intend. The surface is described using a grid like the following:

* SFFF
* FHFH
* FFFH
* HFFG

This grid is our environment where:
* S is the agent’s starting point, and it’s safe.
* F represents the frozen surface and is also safe.
* H represents a hole, and if our agent steps in a hole in the middle of a frozen lake, well, that’s not good.
* Finally, G represents the goal, which is the space on the grid where the prized frisbee is located.

The agent can navigate left, right, up, and down, and the episode ends when the agent reaches the goal or falls in a hole. It receives a reward of one if it reaches the goal, and zero otherwise.
*                                                      State 	  Description 	              Reward
*                                                      S 	Agent’s starting point - safe 	    0
*                                                      F 	Frozen surface - safe 	            0
*                                                      H 	Hole - game over 	            0
*                                                      G 	Goal - game over 	            1 
