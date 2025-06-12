#  Spiral Classification using MLP
This project shows how to sort a tricky 3-class spiral dataset using a Multilayer Perceptron (MLP) made with TensorFlow/Keras. The spiral data has noise and is not straight, which makes it a good test for neural networks.
---
##  Objective
- Create a fake dataset with 3 spiral classes
- Develop, train, and adjust a Multi-Layer Perceptron (MLP) to sort the data
- Show the training progress and decision boundaries
- Think about the model design and how to make it better
---
##  Dataset
The dataset is created with a unique Python function. It forms 3 spiral arms (classes) along with some noise.
- Points in each class: 200
- Overall points: 600
- Noise level: 0.4
- Distribution: 80% for training / 20% for testing
---
##  Model Architecture
- 2D coordinates `(x, y)`
- Hidden Layers: 2
- Layer 1: 32 neurons, using ReLU activation
- Layer 2: 32 neurons, using ReLU activation
- Output Layer: 3 neurons (softmax for classification purposes)
- Loss Function: Categorical Crossentropy
- Optimizer: Adam (with a learning rate of 0.001)
- Total Epochs: 300
- Batch Size: 32
---
##  Training Results
- Graphs illustrate the accuracy and loss for both training and validation
- The decision boundary is depicted to assess the model's performance
- The final model distinctly separates the spiral arms
---
###  Reflection.
 ##  Hidden Layers
Utilized 2 layers featuring 32 neurons — straightforward yet sufficiently robust to grasp spirals.
### Learning Rate
The default setting of 0.001 performed the best; a higher value caused instability, while a lower one resulted in slowness.
### Overfitting
Slight overfitting observed after 300 epochs. This can be enhanced by implementing early stopping or dropout techniques.

### Improvements (Future Work)
- Implement dropout or regularization methods
- Tune hyperparameters
- Introduce learning rate scheduling
- Experiment with different architectures (CNNs, RBFs)
---
## Visuals
- Spiral data plot  
- Accuracy/Loss curves  
- Decision boundary map

## Contact me @ touseefahmed00710@gmail.com.
