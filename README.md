
# Tomato Leaf Disease Classification using InceptionV3

This project implements a deep learning model using the **InceptionV3** architecture to classify tomato plant leaves based on disease. The dataset consists of various classes of tomato leaf diseases and healthy leaves. The model leverages **transfer learning** to achieve high classification accuracy.

## Dataset

The dataset used in this project is the **Tomato Leaf Disease Dataset**, which includes images of tomato leaves classified into the following categories:

- Bacterial Spot
- Early Blight
- Late Blight
- Leaf Mold
- Septoria Leaf Spot
- Spider Mites (Two-Spotted Spider Mite)
- Target Spot
- Tomato Yellow Leaf Curl Virus
- Tomato Mosaic Virus
- Healthy

You can download the dataset from [Kaggle - Tomato Leaf Dataset](https://www.kaggle.com/datasets/kaustubhb999/tomatoleaf) 

## Model Overview

- Architecture: **InceptionV3**
- Technique: **Transfer Learning** using pre-trained ImageNet weights
- Input Shape: 224x224x3 (resized from original)
- Data Augmentation: Yes (rotation, zoom, flip, etc.)
- Optimizer: Adam
- Loss Function: Categorical Crossentropy
- Evaluation Metrics: Accuracy, Confusion Matrix

## Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/tomato-disease-inceptionv3.git
cd tomato-disease-inceptionv3
```

### 2. Prepare the Dataset

Download and unzip the dataset from Kaggle, and arrange the folders as follows:

```
dataset/
├── train/
│   ├── Bacterial_spot/
│   ├── Early_blight/
│   └── ...
├── test/
│   ├── Bacterial_spot/
│   ├── Early_blight/
│   └── ...
```

### 3. Run the Notebook

Open and run the Jupyter Notebook:

```bash
jupyter notebook InceptionV3_Tomato_Dataset.ipynb
```

## Results

- Training Accuracy: ~99%
- Validation Accuracy: ~98%
- Confusion Matrix indicates good performance across all 10 classes.

> Note: Final accuracy may vary depending on the dataset split and number of training epochs.

## License

This project is licensed under the MIT License.

## Acknowledgements

- [Kaggle Dataset - Tomato Leaf Diseases](https://www.kaggle.com/datasets/kaustubhb999/tomatoleaf)
- TensorFlow & Keras Documentation

---
