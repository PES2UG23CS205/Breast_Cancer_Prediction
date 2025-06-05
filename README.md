🩺 Breast Cancer Prediction System

This project presents a Machine Learning-based web application that predicts whether a breast tumor is benign (non-cancerous) or malignant (cancerous) based on diagnostic features derived from digitized images of breast masses.
🔍 Overview

The system uses a Logistic Regression model trained on the Breast Cancer Wisconsin (Diagnostic) Dataset from Kaggle. It allows users to input 30 numeric diagnostic features and receive a prediction result. The app is deployed with:

    🔧 Backend: Flask (Python)

    🎨 Frontend: HTML + Bootstrap

    📈 Model Accuracy: 97.36%

📁 Dataset Description

The dataset consists of 569 instances with 32 columns:

    id: Patient ID

    diagnosis: Target variable (M = Malignant, B = Benign)

The remaining 30 columns are grouped as:

    mean: Average of each feature

    se: Standard error

    worst: Worst (mean of the three largest values)

📊 Feature Explanation

Each feature is computed from a digitized image of a fine needle aspirate (FNA) of a breast mass:
Feature	Description
radius	Distance from center to boundary of cell nuclei
texture	Variation in gray-scale values (contrast)
perimeter	Boundary length of the nucleus
area	Size of the nucleus (in pixels)
smoothness	Local variation in radius lengths
compactness	Perimeter² / Area - 1.0
concavity	Severity of concave portions in the contour
concave points	Number of concave sections of the contour
symmetry	Symmetry of the nucleus
fractal dimension	Complexity of the contour (coastline approximation)

Each of the above 10 features has 3 variants:

    *_mean: Average value

    *_se: Standard error

    *_worst: Maximum (mean of worst 3 values)

🚀 How it Works

    User enters 30 numeric features in the web form.

    Data is passed to the Flask backend.

    Logistic Regression model predicts diagnosis.

    Prediction is returned as "Benign" or "Malignant".

🧠 Learnings

    Applied full ML pipeline: preprocessing, encoding, scaling, training, evaluation.

    Integrated ML with Flask and frontend tools.

    Understood medical data interpretation and real-world applications.

🗂 GitHub Repository

🔗 https://github.com/PES2UG23CS205/Breast_Cancer_Prediction
📌 How to Run Locally

git clone https://github.com/yourusername/Breast_Cancer_Prediction
cd Breast_Cancer_Prediction
pip install -r requirements.txt
python app.py
