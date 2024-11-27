# Fashion-MNIST Classifier Project
TThis project focuses on developing and optimizing a convolutional neural network (CNN) for classifying the Fashion-MNIST dataset. The model incorporates advanced techniques such as data augmentation, regularization, and hyperparameter tuning to achieve strong generalization and performance.

## Problem Statement 

The objective is to classify images of clothing into 10 distinct categories from the Fashion-MNIST dataset. The challenge involves optimizing a CNN architecture to improve accuracy and reduce overfitting, ensuring the model can generalize effectively to unseen data. Key tasks include:

1. Designing and testing different CNN architectures.
2. Incorporating regularization techniques such as dropout and L2 regularization.
3. Applying data augmentation to enhance model generalization.
4. Performing hyperparameter tuning for optimal training performance.

Project Structure
The project was divided into multiple phases for iterative experimentation and improvement.

Experimental Phase:
Initial experiments tested different architectures, hyperparameters, and dataset divisions to identify overfitting and inefficiencies. A simple CNN baseline was used for comparison:
- Baseline Accuracy: 86%
- Baseline Loss: 0.3535

Final Phase:
After addressing overfitting and optimizing the architecture, the final CNN was implemented with:

3 Convolutional Layers with ReLU activation and 3×3 filter sizes.
- Batch Normalization for stabilization.
- Dropout Regularization at 25%.
- Data Augmentation such as rotations and horizontal flips.

*- Final Test Accuracy: 89.76%*

*- Final Test Loss: 0.2874*

## Contents:

- "src/": contains the source code written in Python using TensorFlow/Keras.
  
- "README.md": you are reading it right now!
