🪨✋✌️ Image Classification: Rock Paper Scissors

## 📖 Project Overview

The ImageClassification_RockPaperScissors project aims to build an image classification model capable of recognizing three types of hand gestures — Rock, Paper, and Scissors. This model is developed using a Deep Learning approach based on Convolutional Neural Networks (CNN) to learn visual patterns from images and classify them into the three categories.

## 🎯 Project Goals

1. Implement a CNN model for simple image classification
2. Study model performance on training and validation data
3. Generate a model capable of recognizing hand gestures with high accuracy

## 🧩 Dataset

The dataset used consists of three main classes:
1. Rock
2. Paper
3. Scissors

The dataset is divided into two parts:
1. Training Set → used to train the model
2. Validation Set → used to test model performance after training

## 📊 Data Distribution

The following image shows the total data in each set:

<img width="955" height="204" alt="image" src="https://github.com/user-attachments/assets/e95ed01a-774f-46b1-a1c5-9a6d0a790760" />

## 🖼️ Data Visualization

Before training, visualization of several samples from each class was performed to ensure the data was distributed correctly.

<img width="739" height="448" alt="image" src="https://github.com/user-attachments/assets/40f9e29d-8574-43ba-a904-5a0dba900f59" /> <img width="718" height="445" alt="image" src="https://github.com/user-attachments/assets/dec1fa07-498d-4762-bc1a-7056b612076c" />

## 🧠 Model Architecture

The model is built using Convolutional Neural Networks (CNN) with several main layers:

1. Conv2D for feature extraction from images
2. MaxPooling2D to reduce feature dimensions
3. Flatten to transform extraction results into 1D vectors
4. Dense (Fully Connected Layer) as the final classification layer
5. The model is optimized using Adam optimizer and categorical crossentropy loss function, with accuracy as the main evaluation metric

## ⚙️ Training Process

1. Dataset is read and processed into tensors using ImageDataGenerator
2. Data augmentation is performed to add variation (rotation, flip, zoom, etc.)
3. Model is trained using model.fit() for several epochs
4. Training results are visualized in accuracy and loss graphs

## 🧾 Results and Evaluation

After the model training is completed, testing is performed using new data (testing data).
Here are the model prediction results on several image samples:

<img width="686" height="510" alt="image" src="https://github.com/user-attachments/assets/725dbe74-f484-43d5-96b3-42565cdf5aa6" /> <img width="711" height="523" alt="image" src="https://github.com/user-attachments/assets/bb9739b9-0dcc-4a1a-875e-5df025f7f4a8" />

The model is able to recognize hand gestures with a good accuracy level, especially on data with good lighting quality and clear hand positions.

## 🧪 Model Testing

1. The model is tested with several random images to see if the classification works correctly
2. Each prediction result is accompanied by the actual label and model prediction label for comparison

## 📈 Conclusion

1. The CNN model successfully recognized three classes of hand gestures with high accuracy
2. Model performance can be improved by adding more data or using transfer learning (e.g., with MobileNetV2 or ResNet)
3. This model can serve as a foundation for interactive applications such as games or real-time gesture detection systems using cameras

## 🔧 Technologies Used

1. Python
2. TensorFlow / Keras
3. NumPy & Matplotlib
4. Google Colab / Jupyter Notebook

## 📁 Dataset Information

**Dataset Source**: Rock-Paper-Scissors Images by Julien de la Bruère-Terreault
**License**: CC-BY-SA 4.0
**Total Images**: 2,188 images
- Rock: 726 images
- Paper: 710 images
- Scissors: 752 images

**Image Format**: RGB images, 300x200 pixels, .png format
**Background**: Green background with relatively consistent lighting and white balance

## 🚀 Getting Started

1. Clone this repository
2. Download and extract the dataset
3. Open the Jupyter notebook: `ImageClassification_RockPaperScissors.ipynb`
4. Run the cells sequentially to train and evaluate the model
5. Test the model with your own images

## 📄 License

This project uses the Rock-Paper-Scissors dataset under CC-BY-SA 4.0 license.