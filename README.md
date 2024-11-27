# Fashion-MNIST Classifier Project
TThis project focuses on developing and optimizing a convolutional neural network (CNN) for classifying the Fashion-MNIST dataset. The model incorporates advanced techniques such as data augmentation, regularization, and hyperparameter tuning to achieve strong generalization and performance.

## Problem Statement 

The objective is to classify images of clothing into 10 distinct categories from the Fashion-MNIST dataset. The challenge involves optimizing a CNN architecture to improve accuracy and reduce overfitting, ensuring the model can generalize effectively to unseen data. Key tasks include:

1. Designing and testing different CNN architectures.
2. Incorporating regularization techniques such as dropout and L2 regularization.
3. Applying data augmentation to enhance model generalization.
4. Performing hyperparameter tuning for optimal training performance.

## Project Structure
The project was divided into multiple phases for iterative experimentation and improvement.

### Experimental Phase:
Initial experiments were conducted to refine the CNN architecture and training strategy, addressing issues like overfitting and unstable validation accuracy.

### Final Phase:
The final optimized CNN was implemented with:

- 3 Convolutional Layers with ReLU activation and 3×3 filter sizes.
- Dropout Regularization at 0.25
- Data Augmentation such as rotations and horizontal flips.

*- Final Test Accuracy: 89.76%*

*- Final Test Loss: 0.2874*

### Baseline Model for Comparison:
A simple CNN architecture was implemented as a baseline to evaluate the improvements of the final model. The baseline model included:

- 1 Convolutional Layer with 32 filters of size 2×2 and ReLU activation.
- Max Pooling Layer for down-sampling.
- High Dropout Rate of 60% after pooling and flattening layers, limiting its learning capacity.
- Dense Softmax Output Layer for classifying 10 categories.

Results:
*- Accuracy: 86%*

*- Loss: 0.3535*

The final model significantly outperformed the baseline due to its deeper architecture, balanced dropout, and enhanced regularization techniques.

## Contents:

- "src/": contains the source code written in Python using TensorFlow/Keras.

- "experiment/": includes screenshots of experimental results I got during the tuning phase.
  
- "README.md": you are reading it right now!
