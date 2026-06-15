# CIFAR-10 Image Classification: ANN vs CNN

## Overview
This project demonstrates image classification on the CIFAR-10 dataset and compares the performance of:

- Artificial Neural Network (ANN)
- Convolutional Neural Network (CNN)

The notebook is designed for students and beginners to understand why CNNs outperform traditional ANNs for image-based tasks.

## Dataset
**CIFAR-10** contains:
- 60,000 color images
- Image size: 32 × 32 × 3
- 10 classes:
  - Airplane
  - Automobile
  - Bird
  - Cat
  - Deer
  - Dog
  - Frog
  - Horse
  - Ship
  - Truck

Dataset split:
- Training Images: 50,000
- Test Images: 10,000

## Learning Objectives
- Understand image classification fundamentals.
- Learn image preprocessing techniques.
- Build an ANN model for classification.
- Build a CNN model for classification.
- Compare ANN and CNN performance.
- Understand the importance of convolution and feature extraction.

## Technologies Used
- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib

## Project Workflow

### 1. Load Dataset
Load the CIFAR-10 dataset directly from TensorFlow.

### 2. Data Visualization
Display sample images and corresponding labels.

### 3. Data Preprocessing
- Normalize pixel values from 0–255 to 0–1.
- Flatten images for ANN input.
- Keep image dimensions intact for CNN input.

### 4. ANN Model
Architecture:
- Dense(512, ReLU)
- Dropout(0.3)
- Dense(256, ReLU)
- Dense(10, Softmax)

Characteristics:
- Treats images as flattened vectors.
- Does not preserve spatial information.

### 5. CNN Model
Architecture includes:
- Convolution Layers
- Batch Normalization
- Max Pooling
- Dense Layers
- Softmax Output

Characteristics:
- Preserves spatial relationships.
- Learns hierarchical image features.
- Generally achieves higher accuracy than ANN.

## Model Evaluation
Models are evaluated using:
- Test Accuracy
- Loss
- Performance Comparison

## Expected Outcome
CNN should outperform ANN because:
- CNN extracts local features effectively.
- CNN preserves image structure.
- CNN reduces the number of learnable parameters compared to fully connected networks.

## Repository Structure

```text
.
├── week_4_Dinesh_Jangir_pu.ipynb
├── README.md
```

## How to Run

1. Clone the repository.
2. Install dependencies:

```bash
pip install tensorflow numpy pandas matplotlib
```

3. Open Jupyter Notebook:

```bash
jupyter notebook
```

4. Run all cells in:
   - `week_4_Dinesh_Jangir_pu.ipynb`

## Author
**Dinesh Jangir**

B.Tech Student | Machine Learning Enthusiast

## License
This project is intended for educational and learning purposes.
