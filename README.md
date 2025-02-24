# Cipher Algorithm Detection

This repository contains a machine learning-based approach for identifying cryptographic algorithms from byte sequences. It utilizes various deep learning models, including CNNs, RNNs, and ensemble models, to classify encrypted data.

## 📌 Features
- Supports multiple cryptographic algorithms (e.g., AES-256, DES, RSA, etc.).
- Implements CNN, RNN, and ensemble models for classification.
- Uses Jupyter notebooks for data processing, model training, and evaluation.
- Pre-trained models included for quick testing.

## 💁️ Repository Structure
```
├── README.md                     # Project documentation
├── dataset.ipynb                  # Dataset exploration and preprocessing
├── aboutdataset.ipynb             # Additional dataset insights
├── ensemblemodel.ipynb            # Ensemble model implementation
├── cnnmodel.ipynb                  # CNN-based classification
├── model.ipynb                     # General model training script
├── modelASYMMETRICCNN.h5           # Pre-trained asymmetric CNN model
├── modelasymmetricrnn.h5           # Pre-trained asymmetric RNN model
├── modelcnn.h5                     # Pre-trained CNN model
├── modelstreamcnn.h5               # Pre-trained streaming CNN model
├── modelstreamrnn.h5               # Pre-trained streaming RNN model
├── rnmmodel.h5                     # Pre-trained RNN model
└── rnstream.keras                  # Serialized Keras model
```

## 📊 Dataset
The dataset consists of byte sequences paired with their corresponding encryption algorithm labels. It helps the model learn patterns that distinguish different cryptographic methods.

Example data format:
```json
{
  "byte_sequence": "8b597365180634...",
  "algorithm": "AES-256"
}
```

## 🛠 Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/Narayanan1411/cipher-algorithm-detection.git
   cd cipher-algorithm-detection
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## 🚀 Usage
Run the Jupyter notebooks to explore the dataset and train/test models:
```bash
jupyter notebook
```
Open `ensemblemodel.ipynb` or `cnnmodel.ipynb` to start training.

## 📌 Future Improvements
- Expand the dataset with more encryption algorithms.
- Improve model accuracy with hyperparameter tuning.
- Deploy as a web API for real-time classification.

## 🐜 License
This project is open-source. Feel free to contribute!

