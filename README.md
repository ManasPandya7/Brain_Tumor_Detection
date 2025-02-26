# Brain_Tumor_Detection
This project uses machine learning techniques like Support Vector Machines (SVM) and Logistic Regression for detecting brain tumors from MRI images.

The system processes MRI scans to classify them as either *Positive Tumor* or *No Tumor*

## Dataset
The dataset used in this project is sourced from [Kaggle](https://www.kaggle.com/datasets/sartajbhuvaji/brain-tumor-classification-mri). It contains MRI images categorized into:
- `no_tumor`: Images without tumors.
- `pituitary_tumor`: Images with pituitary tumors.

**Note:** The dataset is not uploaded here due to size constraints. Please download it from Kaggle and place it in the `brain_tumor` folder.


## Installation

Follow these steps to set up the project:

1. Clone this repository:
git clone https://github.com/ManasPandya7/Brain_Tumor_Detection.git


2. Place the dataset in the following structure:

brain_tumor/\
├── Training/\
├── Testing/\
├── Manual/



## Steps in the Workflow

### 1. Data Preparation:
- Images are resized to 200x200 pixels and converted to grayscale.
- Data is split into training and testing sets.

### 2. Feature Scaling:
- Pixel values are normalized between 0 and 1.

### 3. Dimensionality Reduction:
- Principal Component Analysis (PCA) reduces dimensionality while retaining 98% variance.

### 4. Model Training:
- Two models are trained: Logistic Regression and Support Vector Machines (SVM).

### 5. Evaluation:
- Models are evaluated using accuracy metrics on both training and testing datasets.

### 6. Prediction:
- The trained models predict whether a given MRI scan shows a tumor or not.


## Results

| Model                  | Training Accuracy | Testing Accuracy |
|------------------------|-------------------|------------------|
| Logistic Regression    |       100%        |     92.31%       |
| Support Vector Machine |       98%         |     94%          |



## How to Use

1. Open the Jupyter Notebook (`project_brain_tumor_classification.ipynb`).
2. Follow the steps for data loading, preprocessing, training, and evaluation.
3. Use the trained model for predictions on new MRI images.


## Future Improvements
1. Incorporate deep learning models like Convolutional Neural Networks (CNNs).
2. Test on larger datasets for better generalization.
3. Automate hyperparameter tuning for optimal model performance.

---

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Acknowledgments
Special thanks to [Kaggle](https://www.kaggle.com/) for providing the dataset and to Bharati Vidyapeeth Deemed University, Pune, for their guidance and support.

---

