# hand-made-neural-network
Personal challenge : re-code all the components of a deep learning algo (weights, biais, backprop, etc) and benchmark it with the same architecture on keras on a typical example

The code is inspired by the logic of keras, but is much simpler:
  - less features implemented
  - less checks, exceptions, tricky cases allowed, etc.
  - probably much less computionaly efficient

We first focus on a classical dense neural network, with the following features implemented :
  - 5 activation functions:
    - relu, tanh (mostly for hidden layers)
    - linear (for regression output)
    - sigmoid, softmax (for classifiction outputs)
  - 4 loss functions:
    - mse, mae (for regression tasks)
    - binomial crossentropy (for binary classification tasks)
    - multiclass crossentropy (for multiclassification)
  - gradient descent with back-propagation
  - mini-batches
  - simple SGD optimizer only
    - only learning rate adjustable
    - without momentum
 
 
To be coded later :
  - regularization:
     - l1, l2, elasticnet
     - on kernels (weights)
  - metric computation at the end of each batch/epoch for monitoring during training
     - loss functions
     - other metrics (accuracy, roc_auc, etc.)
  - early stopping on validation data
  - training history tracking
  - momentum for SGD optimizer
  
To be coded much later :
  - dropout
  - regularization on biais and activity of the neurons
  - other optimizers
    - rmsprop
    - adam
  
To be never coded :
  - padding
  - CNN specifics:
    - conv2D layers
    - kernels
    - max pooling layers
    - flatting layer
  - RNN specifics:
    - simple RNN layer
    - masking layer
    - LSTM layer
    