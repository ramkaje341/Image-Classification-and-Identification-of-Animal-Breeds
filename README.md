# 🐾 Animal Breed Classifier: Deep Learning 

<div align="center">
  <img src="https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/TensorFlow-2.0%2B-orange?style=for-the-badge&logo=tensorflow&logoColor=white" />
  <img src="https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white" />
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" />
</div>

---

### 📖 Description
This project is an end-to-end **Image Classification** system that identifies specific animal breeds using **Deep Learning**. It features a custom-trained **Convolutional Neural Network (CNN)** and provides a user-friendly interface built with **HTML** and **CSS** for real-time interaction.

### 🌟 Key Features
* **Deep Learning Model:** Built using TensorFlow/Keras for high-accuracy classification.
* **Web Interface:** A responsive frontend allowing users to upload images and view results instantly.
* **Pre-processing:** Automated image resizing and normalization for consistent predictions.
* **Robust Backend:** Integrated using Python (Flask/Django) to handle requests and model inference.

---

## 🛠️ Tech Stack

| Layer | Technology |
| :--- | :--- |
| **Brain (AI)** | Python, TensorFlow, Keras, NumPy |
| **Frontend (UI)** | HTML5, CSS3, Google Fonts |
| **Backend (Server)** | Flask |
| **Image Processing** | OpenCV |

---

## 🚀 How It Works

1.  **User Upload:** The user selects an image of an animal through the web interface.
2.  **Processing:** The image is sent to the backend where it is converted into a numerical array and resized to fit the model input.
3.  **Inference:** The trained **Deep Learning model** analyzes the features (ears, fur pattern, snout shape, etc.).
4.  **Result:** The predicted breed and confidence level are displayed back on the website with custom CSS styling.

---

## 📂 Project Structure
```text
├── static/               # CSS styles and UI images
├── templates/            # HTML files for the web interface
├── models/               # Saved trained model (.h5 or .pkl)
├── app.py                # Main application script
├── train_model.py        # CNN training logic
└── requirements.txt      # List of necessary libraries
```
---
## 💻 Installation & Setup

Follow these steps to get the project running on your local machine:

### 1. Clone the Repository
Open your terminal and run the following commands to download the code:
```bash
git clone [https://github.com/ramkaje341/Image-Classification-and-Identification-of-Animal-Breeds.git]
```
### 2. Install Dependencies
Ensure you have Python installed, then install the required libraries:
pip install -r requirements.txt
### 3. Start the Web Application
Launch the server by running the main application script:
python app.py
### 4. Access the Interface
Once the server is running, open your web browser and navigate to:
URL: http://127.0.0.1:5000
---
## 🧠 Project Workflow

The application follows a structured pipeline to transform a raw image upload into a breed identification:

### 1. Data Preprocessing
Before the image reaches the model, it undergoes several transformations:
* **Resizing:** Images are scaled (e.g., to 224x224 pixels) to match the model's input layer.
* **Normalization:** Pixel values are scaled from [0, 255] to [0, 1] to help the model converge faster.
* **Expansion:** The image is converted into a 4D tensor (Batch Size, Height, Width, Channels).

### 2. The Deep Learning Process
The core of the project is a **Convolutional Neural Network (CNN)** that functions in three main stages:

* **Feature Extraction (Convolutional Layers):** The model scans the image to identify patterns like edges, textures, and shapes (e.g., the shape of an animal's ear or the pattern of its fur).
* **Dimensionality Reduction (Pooling Layers):** These layers reduce the size of the data while keeping the most important information, making the model more efficient.
* **Classification (Fully Connected Layers):** Based on the features extracted, the final layers assign a probability score to each breed.


### 3. Web Interaction (HTML/CSS + Flask)
* The **HTML/CSS** frontend captures the image file.
* The **Flask** backend passes this file to the trained `.h5` model.
* The model returns the prediction, which is then rendered back on the web page for the user.
---
## 👤 Author
   SRIRAM
---
## 📝 License

This project is intended for educational purposes only.
---
