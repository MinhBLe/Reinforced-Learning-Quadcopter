# Reinforced-Learning-Quadcopter
Teach quadcopter to fly using Actor-Critics method

Deep Deterministic Policy Gradients (DDPG) with neural network in Keras:
Actor uses Dense sequence of 300 and 400 with 'relu' activation. 
Critic uses sequence of 300 and 400 for states, and single layer 400 for action with 'relu'. 
Batch normalizarion and L2 regulation to improve learning efficiency and reduce overfitting. 

The Agent combines Actor and Critics networks. Epxeriences are remembered and learned via random samples. 
This random sampling is needed to avoid correlation among sequential samples. 
There are Local and Target entities of each Actor and Critics type with soft update (tau = 0.01). 
