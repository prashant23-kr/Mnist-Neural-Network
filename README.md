# MNIST Neural Network

This project contains a **TensorFlow/Keras implementation of a neural network** that learns to classify handwritten digit images from the famous **MNIST dataset**.

The model is built using a simple feedforward neural network and trained to recognize digits (0–9) with reasonable accuracy.

---

## 📌 Dataset

The MNIST dataset includes:

- 60,000 training images (28×28 grayscale)
- 10,000 test images
- Labels in the range of **0–9**

This dataset is included directly in TensorFlow, so no manual download is required.

---

## 🚀 Project Structure
├── Mnist-Neural-Network.ipynb # The main notebook
├── README.md # This file
├── .gitignore # Git ignore rules
└── LICENSE # Open source license

---

## 🧠 What This Model Does

This neural network:

1. **Normalizes** image pixel values to the range [0, 1]
2. **Flattens** the 2D images into 1D vectors
3. Trains a model with:
   - One hidden Dense layer (128 neurons, ReLU activation)
   - One output Dense layer (10 neurons, Softmax activation)
4. Evaluates accuracy on test data

---

## 📋 Model Architecture

| Layer            | Type         | Output Shape |
|-----------------|--------------|--------------|
| Input           | 28×28 image  | (28, 28)     |
| Flatten         | —            | (784,)       |
| Dense (hidden)  | Fully connected, ReLU | (128,) |
| Dense (output)  | Fully connected, Softmax | (10,) |

---

## 🛠️ Requirements

To run this notebook locally, you need:

- Python 3.7+
- TensorFlow 2.x
- Jupyter Notebook

---

## 💻 Installation & Setup

1. Create a virtual environment (optional but recommended):

   ```bash
   python -m venv venv
   source venv/bin/activate      # macOS/Linux
   .\venv\Scripts\activate       # Windows

2. Install required packages:
3. pip install tensorflow jupyter
Run Jupyter Notebook:

jupyter notebook


Open and run the Mnist-Neural-Network.ipynb file.

📈 Results

When training the model, you will see output similar to:

Epoch 1/10
...
accuracy: 0.8204 - loss: 0.6713


After training, the model is evaluated on the test dataset with:

print(f"Test accuracy: {test_acc:.4f}")


Typical accuracy values are around 80–90% for this simple network.

📌 Notes & Tips

You can improve accuracy by:

Adding more layers

Adding dropout regularization

Using Convolutional Neural Networks (CNNs)

Try visualizing sample images from the dataset and text.


📝 License

This repository is released under the MIT License.

⭐ Credits

Created by prashant23-kr using TensorFlow and Keras.
