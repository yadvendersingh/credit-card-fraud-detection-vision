# Credit Card Fraud Detection using Computer Vision

This project aims to detect credit card fraud using computer vision techniques. The model leverages the MViTv2 Vision Model to classify defaulters, achieving a 20% improvement over traditional techniques.

## Project Structure
 ├── dataset.ipynb
 ├── LICENSE 
 ├── main.ipynb 
 ├── oversample.ipynb 
 ├── README.md


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

1. **Preprocess the Dataset**:
    - Run [dataset.ipynb](http://_vscodecontentref_/5) to preprocess the dataset and generate spectrograms.

2. **Oversample the Data**:
    - Run [oversample.ipynb](http://_vscodecontentref_/6) to balance the dataset using ADASYN.

3. **Train the Model**:
    - Run [main.ipynb](http://_vscodecontentref_/7) to train the MViTv2 Vision Model and evaluate its performance.

## Results

The model achieves a significant improvement in detecting credit card fraud compared to traditional techniques. Detailed metrics and visualizations are provided in the [main.ipynb](http://_vscodecontentref_/8) notebook.

## License

This project is licensed under the MIT License. See the [LICENSE](http://_vscodecontentref_/9) file for details.

## Acknowledgements

- [PyTorch](https://pytorch.org/)
- [timm](https://github.com/rwightman/pytorch-image-models)
- [ADASYN](https://imbalanced-learn.org/stable/references/generated/imblearn.over_sampling.ADASYN.html)
- [Librosa](https://librosa.org/)
- [tqdm](https://tqdm.github.io/)