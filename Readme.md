# 🌱 IoT Based Crop Disease Detection System for Smart Agriculture

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10-blue?logo=python">
  <img src="https://img.shields.io/badge/Flask-Web%20Framework-black?logo=flask">
  <img src="https://img.shields.io/badge/TensorFlow-Deep%20Learning-orange?logo=tensorflow">
  <img src="https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-F7931E?logo=scikitlearn">
  <img src="https://img.shields.io/badge/Arduino-IoT-00979D?logo=arduino">
  <img src="https://img.shields.io/badge/OpenCV-Image%20Processing-green?logo=opencv">
</p>

---

#  Project Overview

The **IoT Based Crop Disease Detection System for Smart Agriculture** is an AI-powered smart farming solution that integrates **Internet of Things (IoT), Machine Learning, and Deep Learning** to monitor crop health and detect plant diseases at an early stage.

The system continuously collects real-time environmental data using IoT sensors connected to an **Arduino Uno**, including:

- 🌡 Temperature
- 💧 Humidity
- 🌱 Soil Moisture

This sensor data is analyzed using **Machine Learning models** such as:

- Random Forest
- XGBoost
- LightGBM

to evaluate crop health and predict disease risk based on environmental conditions.

At the same time, a **USB Camera/Webcam** captures images of crop leaves. These images are processed using a **Convolutional Neural Network (CNN)** trained on the **PlantVillage Dataset** to identify crop diseases and classify plants as **Healthy** or **Diseased** along with a prediction confidence score.

By combining **environmental sensor analysis** with **image-based disease detection**, the system provides farmers with accurate crop monitoring, early disease diagnosis, and intelligent recommendations for precision agriculture.

---

#  Objectives

- Detect crop diseases at an early stage
- Monitor environmental conditions in real time
- Improve farming decisions using Artificial Intelligence
- Reduce crop losses
- Increase agricultural productivity
- Promote precision farming

---

#  Key Features

 Real-time Sensor Monitoring

- Temperature Monitoring
- Humidity Monitoring
- Soil Moisture Monitoring

 AI-Based Disease Detection

- CNN-based leaf image classification
- Disease identification
- Confidence score prediction

 Machine Learning Prediction

- Environmental stress analysis
- Disease risk prediction
- Crop health assessment

 Smart Dashboard

- Live sensor values
- Uploaded leaf image
- Disease prediction
- Risk probability
- Health status
- Farming recommendation

---

# 🛠 Tech Stack

## Programming Languages

- Python
- C/C++ (Arduino)

## Machine Learning

- Scikit-Learn
- Random Forest
- XGBoost
- LightGBM

## Deep Learning

- TensorFlow
- Keras
- CNN (Convolutional Neural Network)

## IoT

- Arduino Uno
- Soil Moisture Sensor
- DHT11 / DHT22 Sensor
- USB Webcam

## Backend

- Flask / FastAPI

## Frontend

- HTML
- CSS
- JavaScript
- Bootstrap

## Libraries

- OpenCV
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-Learn
- TensorFlow
- Joblib

---

#  AI Models Used

## Machine Learning Model

Used for analyzing environmental sensor data.

Algorithms:

- Random Forest
- XGBoost
- LightGBM

### Input

- Temperature
- Humidity
- Soil Moisture

### Output

- Crop Health
- Disease Risk
- Risk Probability

---

## Deep Learning Model

CNN-based model trained on crop leaf images.

### Input

Leaf Image

### Output

- Disease Name
- Healthy/Diseased
- Confidence Score

---

#  Dataset Information

Two publicly available datasets were used in this project.

---

## 1️. Crop Health & Environmental Stress Dataset

Used for Machine Learning model training.

### Contains

- Temperature
- Humidity
- Soil Moisture
- Crop Health
- Environmental Stress

Approximate Records:

**50,000 – 70,000 sensor records**

Dataset Source:

https://www.kaggle.com/datasets/datasetengineer/crop-health-and-environmental-stress-dataset

---

## 2️. PlantVillage Dataset

Used for CNN model training.

Contains thousands of labeled crop leaf images for disease classification.

Approximate Images:

**25,000 – 30,000 images**

Dataset Source:

https://github.com/spMohanty/PlantVillage-Dataset

---

#  System Architecture

```
                     User (Farmer)
                           │
                           ▼
                    Web Application
                           │
        ┌──────────────────┴──────────────────┐
        │                                     │
        ▼                                     ▼
 USB Camera/Webcam                      Arduino Uno
 (Leaf Image)                           │
                                        │
                 ┌──────────────────────┴────────────────────┐
                 │                                            │
          DHT11/DHT22 Sensor                      Soil Moisture Sensor
       (Temperature & Humidity)
                 │
                 ▼
          Flask / FastAPI Backend
                 │
      ┌──────────┴──────────┐
      │                     │
      ▼                     ▼
Image Preprocessing   Sensor Preprocessing
      │                     │
      ▼                     ▼
 CNN Model          Random Forest/XGBoost
      │                     │
      └──────────┬──────────┘
                 ▼
 Disease Prediction &
 Smart Recommendation
                 │
                 ▼
         Results Dashboard
```

---

#  Project Workflow

```text
Start
   │
   ▼
Collect Sensor Data
   │
   ▼
Capture Leaf Image
   │
   ▼
Data Preprocessing
   │
   ├──────────────┐
   │              │
   ▼              ▼
Machine       CNN Model
Learning
   │              │
   └──────┬───────┘
          ▼
Combine Predictions
          │
          ▼
Disease Detection
          │
          ▼
Generate Recommendation
          │
          ▼
Display Results
```

---

#  Project Structure

```
IoT-Based-Crop-Disease-Detection-System/
│
├── backend/
│   ├── app.py
│   ├── routes/
│   ├── models/
│   ├── utils/
│   └── requirements.txt
│
├── frontend/
│   ├── css/
│   ├── js/
│   ├── templates/
│   └── assets/
│
├── datasets/
│   ├── PlantVillage/
│   └── Sensor_Dataset/
│
├── ml_model/
│
├── cnn_model/
│
├── arduino/
│
├── static/
│
├── uploads/
│
├── README.md
│
└── LICENSE
```

---

#  Future Improvements

- Mobile Application
- Cloud Deployment
- SMS Alert System
- Fertilizer Recommendation
- Pest Detection
- Weather Forecast Integration
- Multi-language Support
- GPS-based Farm Monitoring

---

#  Expected Outcomes

- Early Disease Detection
- Improved Crop Yield
- Reduced Farming Costs
- Smart Decision Support
- Sustainable Agriculture
- Precision Farming

---

#  Sample Output

- Sensor Readings
- Leaf Image
- Disease Name
- Confidence Score
- Disease Risk
- Health Status
- Recommendation

---

#  References

### Sensor Dataset

https://www.kaggle.com/datasets/datasetengineer/crop-health-and-environmental-stress-dataset

### PlantVillage Dataset

https://github.com/spMohanty/PlantVillage-Dataset

---

 

#  Support

If you found this project helpful, consider giving it a ⭐ on GitHub.

It motivates us to continue developing AI-powered solutions for smart agriculture.

---

##  License

This project is developed for **academic and research purposes**.

The datasets used in this project belong to their respective owners and are used only for educational and research purposes.