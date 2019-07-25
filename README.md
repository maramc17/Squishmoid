# Squishmoid
- A way to add sparsity to the activation function sigmoid within the SEResNet50 Network, squishmoid takes the function of sigmoid and adjusts the alhpa factor to be a larger number and as it seems the larger that number the more sparse it can become. 

- With the assistance of Xu Ma and Andrew Sansom, I was able to rewrite the code for SEResNet50 with the adjustments of my "Squished" Sigmoid.

- Also Tested was the results of Softmax if the same alpha adjustments were placed but for the softmax function. 

# Results and Findings
The table below shows the testing accuracies for cifar100 and imagenet32, with alpha being at different values.
  > Softmax had sporadic results, making them inefficient compared to the results of sigmoid.

        CIFAR100 RESULTS
        
| Alpha | Test Accuracy | Test Loss |
|-------|---------------|-----------|
|   1   |     74.83     |   ~1.24   |
|   2   |     75.09     |   ~1.23   |
|   5   |     75.82     |   ~1.13   |
