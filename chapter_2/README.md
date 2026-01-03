a structered notes for deep-learning-and-neural-network-by-Michael-Nielsen-2 THE core concept of backpropagation

analogy : "We calculate the error at the end, and then blame the layers backwards to fix the weights." forward -> prediction value backward -> calculated error value

notations

wljk to denote the weight for the connection from the kth neuron in the (l−1)th layer to the jth neuron in the lth layer. blj for the bias of the jth neuron in the lth layer. alj for the activation of the jth neuron in the lth layer

BACKPROPAGATION ALGORITHM

feeding the input vector into the network
activation for the first layer
Loop through every layer
we have to store this vectors at each step to calculate gradient decent
first calculate the error in the "L" th(output) layer
then recursively pass the error by
by Take the error from the layer ahead
Send it backward through the transposed weights
Multiply by the sensitivity of the current layer
then we update the weight and biases based on BP3 and BP4
