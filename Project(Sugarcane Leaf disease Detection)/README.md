# Sugarcane Leaf Disease Detection using Transfer Learning

This project leverages deep learning and transfer learning techniques to detect diseases in sugarcane leaves from images. The solution uses pre-trained convolutional neural networks (CNNs) such as EfficientNet and MobileNet to classify leaf images into their respective disease categories.

## Features

- **Automated Disease Detection:** Classifies sugarcane leaf images into multiple disease categories.
- **Transfer Learning:** Utilizes EfficientNet and MobileNet architectures for high accuracy with limited data.
- **Data Augmentation:** Improves model robustness and generalization.
- **Performance Metrics:** Reports accuracy and F1-score for reliable evaluation.
- **Visualization:** Plots training history for accuracy and loss.

## Dataset

- **Source:** [Kaggle - Sugarcane Leaf Dataset](https://www.kaggle.com/datasets)
- **Structure:** Images are organized in subfolders, each representing a disease class.

## Requirements

- Python 3.7+
- TensorFlow 2.x
- Keras
- NumPy
- Pandas
- Matplotlib
- Seaborn
- scikit-learn

Install dependencies using:
```
pip install tensorflow keras numpy pandas matplotlib seaborn scikit-learn
```

## Usage

1. **Download the Dataset:** Place the dataset in the specified directory (e.g., `/kaggle/input/sugarcane-leaf-disease/Sugarcane Leaf Dataset`).
2. **Run the Notebook:** Execute the notebook cells sequentially to train and evaluate the model.
3. **Model Training:** The notebook supports both EfficientNet and MobileNet architectures. You can switch between them as needed.
4. **Evaluation:** After training, the notebook evaluates the model on a validation set and reports accuracy and F1-score.

## How It Works

- **Data Loading:** Images are loaded and split into training, validation, and test sets.
- **Preprocessing:** Images are resized and normalized.
- **Model Building:** A pre-trained CNN (EfficientNet or MobileNet) is used as the base, with custom dense layers added for classification.
- **Training:** The model is trained with early stopping to prevent overfitting.
- **Evaluation:** The model's performance is measured using accuracy and F1-score.

## Results

- The notebook provides plots for training/validation accuracy and loss.
- Final evaluation metrics (accuracy and F1-score) are printed after testing.

## Customization

- You can adjust the batch size, learning rate, or try different pre-trained models for experimentation.
- The code is modular and easy to adapt for other plant disease datasets.

## License

-MIT

**Note:** This project is for educational and research purposes. For real-world deployment, further validation and testing are recommended.
