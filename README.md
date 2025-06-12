#  Spiral Classification using MLP

This project demonstrates how to classify a challenging 3-class spiral dataset using a Multilayer Perceptron (MLP) built with TensorFlow/Keras. The spiral data is noisy and non-linear, making it a good test for neural networks.

---

##  Objective

- Generate a synthetic 3-class spiral dataset
- Build, train, and tune an MLP to classify the data
- Visualize the training progress and decision boundaries
- Reflect on model design and improvements

---

##  Dataset

The dataset is generated using a custom Python function. It creates 3 spiral arms (classes) with noise.

-  Points per class: 200  
-  Total points: 600  
-  Noise: 0.4  
-  Split: 80% training / 20% testing

---

##  Model Architecture

- Input: 2D coordinates `(x, y)`
- Hidden Layers: 2
  - Layer 1: 32 neurons, ReLU
  - Layer 2: 32 neurons, ReLU
- Output Layer: 3 neurons (softmax for classification)
- Loss: Categorical Crossentropy
- Optimizer: Adam (learning rate = 0.001)
- Epochs: 300
- Batch Size: 32

---

##  Training Results

- Plots show training and validation accuracy/loss
- Decision boundary is visualized to evaluate model performance
- Final model separates spiral arms clearly

---

##  Conclusion.

##  Hidden Layers
Used 2 layers with 32 neurons — simple but powerful enough to learn spirals.

### Learning Rate
Default (0.001) worked best; too high was unstable, too low was slow.

###  Overfitting
Slight overfitting after 300 epochs. Can be improved with early stopping or dropout.

###  Improvements (Future Work)
- Use dropout or regularization
- Hyperparameter tuning
- Add learning rate scheduling
- Try other architectures (CNNs, RBFs)

---

## Visuals

- Spiral data plot  
- Accuracy/Loss curves  
- Decision boundary map

## Contact me @ touseefahmed00710@gmail.com.
