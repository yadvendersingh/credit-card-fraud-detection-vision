# Credit Card Fraud Detection using Computer Vision

This project aims to detect credit card fraud using computer vision techniques. The model leverages the MViTv2 Vision Model to classify defaulters, achieving a 20% improvement over traditional techniques.

## Project Structure
 ```
├── CSV_To_Spectrogram.ipynb
├── LICENSE 
├── Oversample_CSV.ipynb 
├── Training_Inference.ipynb 
├── README.md
├── requirements.txt
```

## Notebooks

- **dataset.ipynb**: Preprocesses the dataset, converts audio signals to spectrograms, and splits the data into training and validation sets.
- **main.ipynb**: Trains the MViTv2 Vision Model using the preprocessed dataset and evaluates its performance.
- **oversample.ipynb**: Balances the dataset using ADASYN to handle class imbalance.

## Setup

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/credit-card-fraud-detection-vision.git
    cd credit-card-fraud-detection-vision
    ```

2. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```

3. Download the dataset and place it in the appropriate directory.

4. Run Oversample_CSV.ipynb to balance the classes.

5. Run CSV_To_Spectrogram.ipynb to convert the textual data to Spectrogram.

6. Run Training_Inference.ipynb to train and evaluate the model.

## Usage

1. **Preprocess and Oversample the Dataset**:
    - Run [Oversample_CSV.ipynb](https://github.com/yadvendersingh/credit-card-fraud-detection-vision/blob/main/Oversample_CSV.ipynb) to preprocess the dataset and balance the classes.

2. **Convert to Spectrogram**:
    - Run [CSV_To_Spectrogram.ipynb](https://github.com/yadvendersingh/credit-card-fraud-detection-vision/blob/main/CSV_To_Spectrogram.ipynb) to convert the numeric features to spectrogram.

3. **Train the Model and Inference**:
    - Run [Training_Inference.ipynb](https://github.com/yadvendersingh/credit-card-fraud-detection-vision/blob/main/Training_Inference.ipynb) to train the MViTv2 Vision Model and evaluate its performance.

## Results

The model achieves a significant improvement in detecting credit card fraud compared to traditional techniques with ~19% improvement over XGBoost and Logistic Regression models and achieving 96.97% ROC AUC score

## License

This project is licensed under the MIT License. See the [LICENSE](https://github.com/yadvendersingh/credit-card-fraud-detection-vision/blob/main/LICENSE) file for details.

## Acknowledgements

- [PyTorch](https://pytorch.org/)
- [timm](https://github.com/rwightman/pytorch-image-models)
- [ADASYN](https://imbalanced-learn.org/stable/references/generated/imblearn.over_sampling.ADASYN.html)
- [Librosa](https://librosa.org/)
- [tqdm](https://tqdm.github.io/)
- [Kaggle Dataset - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud/data/)
