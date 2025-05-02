🔥 Fire Detection using MobileNetV2
This project implements a deep learning model for real-time fire detection using MobileNetV2, a lightweight convolutional neural network optimized for mobile and embedded vision applications. The model is trained to classify images as either fire or non-fire.

📁 Dataset Structure
Place your dataset in the following structure:
dataset/
├── train/
│   ├── fire/
│   └── non_fire/
├── test/
│   ├── fire/
│   └── non_fire/


🧠 Model Architecture
Base model: MobileNetV2 (with pre-trained ImageNet weights)

Preprocessing: Keras ImageDataGenerator with data augmentation

Optimizer: Adam

Input Size: 224x224 pixels

🛠️ Dependencies
Install the required libraries: pip install tensorflow

🚀 Training the Model
The notebook automatically:

Loads and preprocesses training/testing data

Builds a MobileNetV2-based classifier

Trains the model on the training set

Evaluates it on the test set

🧪 Evaluation
The model reports accuracy and loss on the test dataset after training. Optionally, you can add confusion matrix and classification reports for deeper insight.

💾 Saving & Loading
Modify the notebook to save your trained model using:

model.save('fire_detection_model.h5')
And load it later with:


model = keras.models.load_model('fire_detection_model.h5')
📌 Notes
Ensure you have a balanced dataset.

Use a GPU-enabled environment for faster training.

