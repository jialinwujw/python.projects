# About The Analysis
This project utilizes a dataset of blood smear images to perform malaria detection.<br>
It classifies blood smears into two categories: parasitized (infected with the malaria parasite Plasmodium) and uninfected (normal, uninfected red blood cells).<br>
The primary goal is to assist in automated malaria diagnosis.

## Project
[Python code HTML version](https://htmlpreview.github.io/?https://github.com/jialinwujw/python.projects/blob/main/medical_image_analysis/medical_image_analysis.html)

### Data
https://www.tensorflow.org/datasets/catalog/malaria

### Description
The dataset used in this project is sourced from the TensorFlow dataset collection and consists of 27,558 labeled cell images of blood smears. It is divided into two classes:

- Parasitized: Images of blood smears containing red blood cells infected with the malaria parasite Plasmodium.
- Uninfected: Images of blood smears containing normal, uninfected red blood cells.

### Python Packages
* numpy
* matplotlib
* tensorflow

```sh
import numpy as np
import matplotlib.pyplot as plt
import tensorflow as tf
from tensorflow import keras
import tensorflow_datasets as tfds
```

### Methodology
My approach to malaria detection follows a structured methodology to ensure reliable results:

1. **Data Preprocessing**:
   - Images are resized to a uniform 64x64 pixel size and pixel values are normalized.

2. **Model Selection**:
   - I leverage a pre-trained VGG16 architecture as a feature extractor to capture informative image features.

3. **Custom Classification Layers**:
   - Custom classification layers are added to the model, including Dense layers with ReLU activation, BatchNormalization, and Dropout for regularization.

4. **Model Training**:
   - The model is trained on a split dataset using sparse categorical cross-entropy loss and the Adam optimizer with a learning rate of 1e-4.
   - Early stopping is implemented to mitigate overfitting.

5. **Evaluation**:
   - I evaluate the model's performance on the test dataset and print the test loss and accuracy.

### Results

The final model achieved a test accuracy of approximately 96.08%, demonstrating its effectiveness in malaria detection.
