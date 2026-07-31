🌿 Plant Disease Detection using CNN

A Convolutional Neural Network (CNN) built with TensorFlow/Keras to classify plant leaf images as healthy or diseased, across 38 classes covering multiple crop species (Apple, Corn, Tomato, Grape, Potato, etc.).

📊 Overview

Dataset: [PlantVillage Dataset](https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset) (Kaggle) — ~57,000 labeled leaf images
Model: Sequential CNN (3 convolutional blocks + fully connected layers)
Input size: 224x224 RGB images
Framework: TensorFlow / Keras

🎯 Results

| Metric | Score |
|---|---|
| Training Accuracy | 99.75% |
| Validation Accuracy | 90.45% |

🧠 Model Architecture

- 3x `Conv2D` + `MaxPooling2D` blocks (feature extraction)
- Fully connected `Dense` layers for classification
- Optimizer: `Adam`
- Loss: `categorical_crossentropy`

📁 Project Structure


plant-disease-detection-cnn/
├── Plant_Disease_Detection_using_CNN.ipynb   # Main notebook
├── README.md
└── .gitignore


🚀 How to Run

1. Open the notebook in [Google Colab](https://colab.research.google.com/)
2. Get a Kaggle API key (`kaggle.json`) from your [Kaggle account settings](https://www.kaggle.com/settings) → API → Create New Token
3. Run the notebook cells in order — it will:
   - Prompt you to upload `kaggle.json`
   - Download the PlantVillage dataset automatically
   - Train the CNN model
   - Let you upload a leaf image for prediction

🛠️ Requirements

- Python 3.x
- TensorFlow / Keras
- NumPy, Pandas, Matplotlib, OpenCV
- Kaggle API (`kaggle` package)

📌 Notes

- The dataset (~2GB) and trained model weights are **not included** in this repo — download the dataset via Kaggle as shown above.
- Keep your `kaggle.json` private; never commit it to GitHub.

📄 License

This project is open source and available for educational use.
