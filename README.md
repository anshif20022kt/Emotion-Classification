# Emotion Classification using Support Vector Machine (SVM)

This project implements an emotion classification system using a Support Vector Machine (SVM) model. The system is designed to classify input features (e.g., speech or text embeddings) into distinct emotion categories. The implementation includes data preprocessing, model training, evaluation, and performance reporting.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/emotion-svm-classifier.git
   cd emotion-svm-classifier
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

   **Required packages** may include:
   - `scikit-learn`
   - `pandas`
   - `numpy`
   - `matplotlib` *(for plotting if used)*

## Usage

Run the script using Python:

```bash
python svm_emotion_classification.py
```

**Input Format:**  
The script expects a CSV file with features and labels. Update the file path in the script accordingly.

Example structure of CSV:
```
feature1, feature2, ..., featureN, label
```

## Dataset

The dataset should contain pre-extracted features representing input data (e.g., MFCCs for speech or embeddings for text) and corresponding emotion labels.

You can use datasets like:
- [RAVDESS (Ryerson Audio-Visual Database of Emotional Speech and Song)](https://zenodo.org/record/1188976)
- [CREMA-D](https://github.com/CheyneyComputerScience/CREMA-D)
- [EmotionText Dataset](https://www.kaggle.com/datasets/praveengovi/emotions-dataset-for-nlp)

Make sure to format your dataset correctly before using.

## Model Description

- **Classifier:** Support Vector Machine (SVM)
- **Kernel:** Default (`rbf`) or customizable
- **Preprocessing:** Standardization of features using `StandardScaler`
- **Train/Test Split:** 70/30 or configurable

## Evaluation Metrics

The script computes:
- Accuracy
- Precision, Recall, F1-score
- Confusion Matrix

These metrics help evaluate how well the model classifies each emotion.

## Results

Example output:
```
Accuracy: 85.3%
F1 Score: 0.84
Classification Report:
  precision    recall  f1-score   support

     happy       0.86      0.84      0.85        50
       sad       0.82      0.86      0.84        50
   neutral       0.87      0.84      0.85        50
```

*Note: Your actual results will vary based on the dataset used.*

## Author

- Team: [MUHAMMED ANSHIF KT]
- Contact: [muhammedkt.ds24@duk.ac.in]

## License

This project is open source and available under the [MIT License](LICENSE).
