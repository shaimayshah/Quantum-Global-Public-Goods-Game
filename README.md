This project refers to the following issue : https://github.com/qiskit-community/qiskit-camp-asia-19/issues/13

# Abstract
The well-being of our global ecosystem is dependent on the shared preservation of global public goods (GPGs). A GPG is a good which cannot be replaced with any other good, and that no one can be theoretically excluded from, such as air or climate change impact. One of the biggest threats to GPG integrity is the free-rider problem, which is a well defined problem in Game theory frame. Is it possible to develop another approach of this issue using quantum entanglement and hence demonstrate on a valuable problem quantum advantage? The answer seems to be yes and it might be possible to show it on a simple case building an efficient algorithm in Qiskit.



# How to use

Our framework optimize a given cost function by finding the corresponding strategy for each player.
The payoff matrix is of size <a href="https://www.codecogs.com/eqnedit.php?latex=$2^n&space;\times&space;n$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$2^n&space;\times&space;n$" title="$2^n \times n$" /></a>, each column is representing the payoff of a player for each strategy.
A cost function must also be provided, it map the payoff vector to a relevent quantity to optimize.

![circuit](circuit.png)

In the circuit above, the inputs are <a href="https://www.codecogs.com/eqnedit.php?latex=$\phi_i$,&space;$\theta_i$,&space;$\lambda_i$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$\phi_i$,&space;$\theta_i$,&space;$\lambda_i$" title="$\phi_i$, $\theta_i$, $\lambda_i$" /></a>, this input represent the initial strategy for the player <a href="https://www.codecogs.com/eqnedit.php?latex=$i$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$i$" title="$i$" /></a>.

In our program these values are set in a vector of named input, we have <a href="https://www.codecogs.com/eqnedit.php?latex=$input&space;=&space;\[\phi_1,&space;\theta_1,&space;lambda_1,&space;...,&space;\phi_n,&space;\theta_n,&space;lambda_n\]$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$input&space;=&space;\[\phi_1,&space;\theta_1,&space;\lambda_1,&space;...,&space;\phi_n,&space;\theta_n,&space;\lambda_n\]$" title="$input = \[\phi_1, \theta_1, lambda_1, ..., \phi_n, \theta_n, lambda_n\]$" /></a> where <a href="https://www.codecogs.com/eqnedit.php?latex=$n$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$n$" title="$n$" /></a> is the number of players.


Our framework also works for classical strategies.
In this case only one input per player is needed, <a href="https://www.codecogs.com/eqnedit.php?latex=$input&space;=&space;\[\theta_1,&space;...,&space;\theta_n&space;\]$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$input&space;=&space;\[\theta_1,&space;...,&space;\theta_n&space;\]$" title="$input = \[\theta_1, ..., \theta_n \]$" /></a> where <a href="https://www.codecogs.com/eqnedit.php?latex=$n$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$n$" title="$n$" /></a> is the number of players.

