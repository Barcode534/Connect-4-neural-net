# Connect-4-neural-net

This is my connect four deep neural network AI, using Q learning.

Based on Axiomatic Uncertainty's code, I changed the the game to connect 4. Tic Tac Toe has 5k game states, whereas C4 has 3.5 trillion.

There is a lot of experimentation required when testing a neural network. The epsilon greedy values, learning rate, number of hidden layers and number of neurons. 

This current code does ''learn'' how to play, but it will still lose eventually versus strong play. Of course, with more training (possibly on google cloud/AWS) it will get better. 

Having been to a talk on NNs for NLP, I think this NN is unnecessarily large. I now think the original TTT was too large, but when I started this challenge I felt like imcreasing the size of the NN was logical. What I am worried is happening is the AI is learning every game state by trial and error / monte carlo simulations, which is NOT the objective of this program.

On the one hand, it's ok because computers are very good at simulating mass events and determing best action from this experience, but on the other hand, humans know immediately that getting/blocking a general 2-3-4 in a row is a strong strategy. Even before a single move is made.

Then again, how else will a computer learn unless it's trial and error, given that we do not want to code in rules such as ''try to make 2 in a row, then 3 in a row, then 4 in a row. Whilst blocking opponents 4 in a row''.

Anyway, I am going try a smaller neural network and hope it picks up on general patterns of play faster.

I do not want the large neural network to overfit to many unique situations. I want a simple NN that can play all games states of C4 to a high level.
