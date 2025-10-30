🧠 CNN Classifier – Dogs vs Cats 🐶🐱

A Convolutional Neural Network (CNN) built with TensorFlow/Keras to classify images of dogs and cats using the Kaggle Dogs vs. Cats dataset.
The model is trained end-to-end on augmented image data and achieves strong performance on this binary classification task.

🚀 Features

Downloads the dataset directly from Kaggle using the Kaggle API

Automatically unzips and organizes the dataset into training and validation folders

Applies data augmentation techniques for better generalization

Builds and trains a CNN architecture using TensorFlow/Keras

Allows real-time prediction on custom images

Includes validation accuracy tracking during training

🧩 Model Architecture

The CNN consists of:

Layer Type	Filters/Units	Kernel Size	Activation	Additional Info
Conv2D	32	3x3	ReLU	Input shape (150,150,3)
MaxPooling2D	—	2x2	—	—
Conv2D	64	3x3	ReLU	—
MaxPooling2D	—	2x2	—	—
Conv2D	128	3x3	ReLU	—
MaxPooling2D	—	2x2	—	—
Flatten	—	—	—	—
Dense	512	—	ReLU	Fully Connected Layer
Dense	1	—	Sigmoid	Output Layer (Binary)
📦 Requirements

Install the dependencies using pip:

pip install tensorflow kaggle numpy


You also need your Kaggle API key (kaggle.json).

⚙️ Setup Instructions

Clone this repository

git clone https://github.com/yourusername/cnn-dog-cat-classifier.git
cd cnn-dog-cat-classifier


Add your Kaggle API key

Download kaggle.json from your Kaggle account settings.

Place it in the project root folder.

Run the script

python cnn_classifier_example.py


This will:

Set up Kaggle authentication

Download and unzip the dataset

Train the CNN model

Print predictions for a test image

🧠 Training Details

Optimizer: Adam

Loss: Binary Crossentropy

Metrics: Accuracy

Epochs: 10

Image size: 150×150

Batch size: 32

Validation Split: 20%

🔮 Prediction Example

To predict a custom image, place it in the project directory as image.jpg and run:

python cnn_classifier_example.py


Output Example:

0.8723
Dog 🐕

📊 Results
Metric	Value
Training Accuracy	~90%
Validation Accuracy	~85% (varies slightly)
📁 Project Structure
cnn_classifier_example.py
kaggle.json
data/
├── train/
│   ├── cats/
│   └── dogs/
test/
└── test1/

🧑‍💻 Author

Prabhat Jain
B.S. Economics (Minor in Data Science), IISER Bhopal
GitHub:github.com/prabhatj228-lab
