# Tumor Detection using CNN

![Tumor Detection App - a Hugging Face Space by annapurnapadmaprema-ji - Google Chrome 16-11-2024 02_04_55 PM](https://github.com/user-attachments/assets/04cac903-ee60-4d10-bfec-72c7a4b751b4)



This project is a web-based application for detecting tumors in medical images using a pre-trained Convolutional Neural Network (CNN). It provides an intuitive interface for users to upload images and receive predictions.
Visit project to know more : https://huggingface.co/spaces/annapurnapadmaprema-ji/Tumor-Detection-App![Uploading Tumor Detection App - a Hugging Face Space by annapurnapadmaprema-ji - Google Chrome 16-11-2024 02_04_55 PM.png…]()

## Application Overview
- **Upload an Image**: Supports medical images in `.jpg`, `.jpeg`, or `.png` format.
- **Real-Time Predictions**: Classifies images as either "Tumorous" or "Non-tumorous."
- **Visual Feedback**: Displays the uploaded image along with the prediction result.

## Model Details
- The **CNN model** (`cnn_tumor2.h5`) is trained on a dataset of medical images for binary classification.
- Input images are resized to `128x128` pixels and normalized for consistency during prediction.
- The model uses a probability threshold of **0.5**:
  - Predictions > 0.5 are classified as **"Tumorous"**.
  - Predictions ≤ 0.5 are classified as **"Non-tumorous"**.

## How It Works
1. Users upload a medical image.
2. The image is preprocessed by resizing and normalization.
3. The preprocessed image is passed through the trained CNN model.
4. The application displays the classification result based on the model's prediction.
