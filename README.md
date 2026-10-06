# Skin Cancer Detection

A machine learning project for analyzing skin lesion images and assisting in skin cancer classification.

## Overview

This project uses Python and machine learning/computer vision techniques to process skin lesion images and build a classification model.

The main implementation is available in `Skin_Cancer_Detection.ipynb`.

## Technologies

- Python
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- TensorFlow & Keras

## Getting Started

Clone the repository:

```bash
git clone https://github.com/Ashish8873/Skin-Cancer.git
cd Skin-Cancer
```

Open the notebook:

```bash
jupyter notebook Skin_Cancer_Detection.ipynb
```

Install the libraries required by the notebook before running it.

## Implementation
The notebook creates a CNN model. And then it is trained on [MNIST Dataset]("https://www.kaggle.com/kmader/skin-cancer-mnist-ham10000").

Model Summary
```
Model: "sequential_2"
_________________________________________________________________
 Layer (type)                Output Shape              Param #
=================================================================
 conv2d_10 (Conv2D)          (None, 28, 28, 16)        448

 max_pooling2d_4 (MaxPooling  (None, 14, 14, 16)       0
 2D)

 batch_normalization_12 (Bat  (None, 14, 14, 16)       64
 chNormalization)

 conv2d_11 (Conv2D)          (None, 12, 12, 32)        4640

 conv2d_12 (Conv2D)          (None, 10, 10, 64)        18496

 max_pooling2d_5 (MaxPooling  (None, 5, 5, 64)         0
 2D)

 batch_normalization_13 (Bat  (None, 5, 5, 64)         256
 chNormalization)

 conv2d_13 (Conv2D)          (None, 3, 3, 128)         73856

 conv2d_14 (Conv2D)          (None, 1, 1, 256)         295168

 flatten_2 (Flatten)         (None, 256)               0

 dropout_6 (Dropout)         (None, 256)               0

 dense_10 (Dense)            (None, 256)               65792

 batch_normalization_14 (Bat  (None, 256)              1024
 chNormalization)

 dropout_7 (Dropout)         (None, 256)               0

 dense_11 (Dense)            (None, 128)               32896

 batch_normalization_15 (Bat  (None, 128)              512
 chNormalization)

 dense_12 (Dense)            (None, 64)                8256

 batch_normalization_16 (Bat  (None, 64)               256
 chNormalization)

 dropout_8 (Dropout)         (None, 64)                0

 dense_13 (Dense)            (None, 32)                2080

 batch_normalization_17 (Bat  (None, 32)               128
 chNormalization)

 dense_14 (Dense)            (None, 7)                 231

=================================================================
Total params: 504,103
Trainable params: 502,983
Non-trainable params: 1,120
_________________________________________________________________
```

## Disclaimer

This project is for educational and research purposes only. It is not a medical diagnostic tool and should not replace professional medical advice.

## License

This project is released under the Unlicense.

## Author

Ashish Kumar
