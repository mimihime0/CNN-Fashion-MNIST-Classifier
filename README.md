# Fashion-MNIST CNN Classifier 

## Description

This project implements and optimizes a Convolutional Neural Network (CNN) using Python with TensorFlow/Keras within a Jupyter Notebook environment to classify images from the popular Fashion-MNIST dataset. The goal is to accurately categorize grayscale images of clothing items (like T-shirts, trousers, dresses, etc.) into 10 distinct classes.

The development process involved iterative experimentation, focusing on optimizing the CNN architecture and training process by incorporating techniques like data augmentation and regularization (Dropout, L2) to improve accuracy and generalization on unseen data. A baseline model is also included for performance comparison.

## Features

* Image classification for the Fashion-MNIST dataset (10 clothing categories).
* Implementation of Convolutional Neural Networks (CNNs).
* Use of advanced techniques during development:
    * Data Augmentation (e.g., rotations, flips) to improve robustness.
    * Regularization (Dropout, potentially L2) to reduce overfitting.
    * Hyperparameter tuning exploration (details likely in `experiment/`).
* Includes both an optimized final model and a simpler baseline model for comparison.
* Reports final test accuracy and loss metrics within the notebook output.

## Requirements

* Python (likely 3.7+)
* TensorFlow (`tensorflow`)
* NumPy (`numpy`)
* (Potentially) Matplotlib (`matplotlib`) for visualizing results or data.
* A Jupyter Notebook environment (e.g., Jupyter Lab, Jupyter Notebook, Google Colab, VS Code with Jupyter extension).

You can typically install the required Python packages using pip:

```bash
pip install tensorflow numpy matplotlib jupyterlab notebook
```

## Model Details

The project involved experimenting with different CNN architectures. The key models are:

### Final Optimized Model

This model represents the outcome of optimization efforts, incorporating deeper layers and regularization techniques.

* **Architecture:**
    * 3 Convolutional Layers (using 3x3 filters, ReLU activation).
    * Likely includes Max Pooling layers after convolutional layers (common practice).
    * Flatten layer before dense layers.
    * Dense output layer with Softmax activation (for 10 classes).
* **Regularization:**
    * Dropout applied (rate specified as 0.25).
    * (Potentially L2 regularization, as mentioned in the problem statement).
* **Data Augmentation:**
    * Techniques like random rotations and horizontal flips were applied during training.

### Baseline Model

A simpler CNN used for comparison to demonstrate the effectiveness of the optimizations.

* **Architecture:**
    * 1 Convolutional Layer (32 filters, 2x2 size, ReLU activation).
    * 1 Max Pooling Layer.
    * Flatten layer.
    * Dense output layer with Softmax activation (10 classes).
* **Regularization:**
    * High Dropout Rate (specified as 60%) applied after pooling and flattening.

## Usage

1.  Ensure you have Python and the required libraries installed (see Requirements).
2.  Make sure you have a Jupyter Notebook environment set up.
3.  Navigate to the project directory in your terminal.
4.  Start your Jupyter environment (e.g., run `jupyter lab` or `jupyter notebook`).
5.  Open the `.ipynb` notebook file located in the `src/` directory within the Jupyter interface.
6.  Run the cells in the notebook sequentially to load data, define models, train, evaluate, and view results.

## Results

Performance comparison between the final optimized model and the baseline (as observed in the notebook output):

* **Final Model:**
    * Test Accuracy: **89.76%**
    * Test Loss: **0.2874**
* **Baseline Model:**
    * Test Accuracy: 86%
    * Test Loss: 0.3535

The final model demonstrated improved accuracy and lower loss compared to the baseline, highlighting the benefits of the deeper architecture, data augmentation, and refined regularization.
