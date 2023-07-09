## First Attempt 

In my first attempt I just used the configurations shown in the lecture, with the focus on just getting a working model at first as well as setting a baseline for future tests
 Average Epoch = 6s
 Final Loss = 3.6711
 Final Accuracy = 0.05616

Baseline Layers
* 32 filters
* Max-pooling layer using 2x2 pool size
* Flatten units
* Hidden layer with 128 nodes and 0.5 dropout
* Output layer using softmax activation

## Second Attempt (100 Convolutions)

Second attempt we changed the first convolutional layer from 32 to 100
 Average Epoch = 12s
 Final Loss = 3.5
 Final Accuracy = 0.055

* Increased time per epoch, no significant change in loss or accuracy

## Third Attempt 300 nodes in the first hidden layer

Third attempt we added 300 nodes in the hidden layer instead
 Average Epoch = 17s
 Final Loss = 0.9096
 Final Accuracy = 0.7249

 * Increased time per epoch
 * Reduced loss
 * Increased accuracy

 ## Fourth Attempt 300 nodes in the first hidden layer + another 100 nodes layer
 Average Epoch = 32s
 Final Loss = 3.5028
 Final Accuracy = 0.0567

* Interestingly this model performed worse than the previous, the new layer added a bit more noise which reduced the accuracy of the original 


## Fifth Removed 300 and 100 nodes, added 10x layers each 10 nodes each (deeper net)
Average Epoch = 8ms
Final Loss = 3.5
Final Accuracy = 0.05 
