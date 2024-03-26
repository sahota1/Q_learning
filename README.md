# Q_learning
1 Review of Q learning and Cart-pole System
Tabular Q learning:
Q learning is an algorithm that relies on updating its state-action value functions.
CartPole environment
The Cart-Pole consists of a pole, which is connected to a horizontally moving cart. To
solve the task, the pole has to be balanced by applying a force F to the cart. The system

CartPole environment
The Cart-Pole consists of a pole, which is connected to a horizontally moving cart. To
solve the task, the pole has to be balanced by applying a force F to the cart. The system
Figure 1: Cartpole System.
is nonlinear since the rotation of the pole introduces trigonometric functions into the force
balance equations. Furthermore, the system’s equilibrium with the pole in the up-right
position is unstable, as small disturbances will cause the pole to swing down. The states
of the Cart-Pole system are the distance s of the cart, the velocity v = ˙s of the cart, the
angle of the pole θ, and the angular velocity of the pole ˙θ. The parameters of the system
include mp - the mass of the pole, mk - the mass of the cart, and Jp - the moment of
inertia for the pole. The dynamics of the Cart-Pole are discussed in Lecture 13 (please
check out the lecture note for more details). Based on the model, one can derive a linear
approximation model around the equilibrium point and design a model-based controller.
In this assignment, we consider the parameters of the system, i.e., mp, mk, Jp are unknown
thus we need to implement a model-free controller, using Q-learning.
