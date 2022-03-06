# Training AI model to play Flappy Bird

. Tools used: Pygame(for developing the game interface), Python NEAT (Neuro Evolution of Augmenting Topologies)

## NEAT Algorithm Process: 

1. `Inputs`: Bird Y (Position of bird on y axis), Top Pipe (position of Top Pipe), Bottom Pipe (position of Bottom Pipe)
2. `Output` : Whether to make the bird jump or not jump
3. `Activation Function` : TanH
4. `Population Size` : 10 Birds (can take any larger number, but taking larger size will overfit the model, as it's a very small game)
5. `Fitness Function` : The fitness of the Bird is dependent upon how long it plays the game (how far it can go)
6. `Maximum Generations` : 30, After running 30 Generations, if the Algorithm couldn't crack the game, then it means it failed(in our test case)

*How the birds are trained in each generation?* : 
###### In 1st Gen, 10 random birds will be played, then the best among them will be choosen and mutated and populated with the next generation birds.
