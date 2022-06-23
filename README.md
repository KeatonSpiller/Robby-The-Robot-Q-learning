# Robby-The-Robot-Q-learning
AI Reinforcement Learning Using Q Learning
* Python version 3.10 or higher
* Jupyter
1. Load the libraries numpy, matplotlib, and scikit-learn 

2. Change the Hyper parameters below 

N = 5000 # Number of Episodes
M = 200 # number of actions to perform in each episode
epsilon = 0.1 # Can start with high ε, and decrease it over the run
eta = 0.2
gamma = 0.9

decreasing_epsilon = True # Change this to be False to have constant epsilon
action_tax = False # Change this to be true to have a -5 action tax

3. Train the model 
run This code:
training_reward, trained_Q_Matrix = Q_Learning_Robby(N, M, epsilon, eta, gamma, decreasing_epsilon, Q_Matrix, action_tax)

4. Test the model
run This code:
test_reward, tested_Q_Matrix = Q_Learning_Robby(N, M, epsilon, eta, gamma, False, trained_Q_Matrix, action_tax)

The Neural Network attempt is in it's own section, it re uses some of the code from above and is ran the same way
It's hyper parameters use a smaller number of episodes because of the time to train each seperate neural network
