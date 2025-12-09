🌿 AI-Powered Ensemble Deep Learning Framework for Plant Disease Detection

This project presents an intelligent, ensemble-based deep learning system designed to detect tea leaf diseases using a hybrid combination of CNN, DenseNet121, and VGG16. The framework improves prediction stability, accuracy, and robustness by leveraging complementary feature extraction capabilities of multiple architectures.

The final triple-model ensemble achieves 81.39% accuracy, outperforming all single and dual-model combinations. The system is deployed using Streamlit, allowing real-time and user-friendly disease prediction.

🚀 Features

✔️ Ensemble deep learning framework (CNN + DenseNet121 + VGG16)

✔️ Real-time disease classification using Streamlit

✔️ Automated preprocessing (resizing, normalization, augmentation)

✔️ Weighted ensemble fusion for improved accuracy

✔️ Supports six tea leaf classes

✔️ Advisory module with precautionary suggestions

✔️ Well-calibrated predictions using Platt Scaling / Isotonic Regression

📂 Dataset

The project uses the TeaLeafBD dataset (Kaggle) containing six classes:

Class	Count
Healthy Leaf	745
Red Leaf Spot	701
Gray Blight	682
White Spot	703
Pest-Infected Leaf	744
Algal Leaf Disease	654

Images contain real-world variations in lighting, noise, and orientation.

🛠️ Methodology
1. Preprocessing

Resize images to 224×224

Normalize pixel values (0–1)

Data augmentation (rotation, zoom, flip, brightness)

Class rebalancing

2. Models Used

CNN (Custom)

DenseNet121 (Transfer Learning)

VGG16 (Transfer Learning)
Each model outputs class probability scores.

3. Ensemble Pipeline

All model permutations tested:

3 single models

3 dual-model ensembles

1 triple-model ensemble

Final fusion uses weighted soft voting.

4. Deployment

Streamlit-based UI

Real-time prediction

Displays confidence scores & disease name

Advisory system triggers if confidence ≥ 0.80

📊 Results
Model	Accuracy
CNN	69.80%
DenseNet121	70.09%
VGG16	77.87%
CNN + DenseNet	76.45%
CNN + VGG16	78.73%
DenseNet + VGG16	80.44%
CNN + DenseNet + VGG16	81.39% (Best)

▶️ Running the Project
1. Install dependencies
pip install -r requirements.txt

2. Run Streamlit app
streamlit run streamlit_app.py

3. Upload an image

The system predicts:

Disease Name

Confidence Score

Severity Level

Recommended Actions

📱 Future Work

Mobile app deployment (TensorFlow Lite)

Multi-crop and multi-disease expansion

Drone-based aerial leaf disease detection

Explainable AI using Grad-CAM

📘 Citation / Reference for Your Project Report

If someone uses your project, they may cite it as:

Mecharla, P. (2025). AI-Powered Ensemble Deep Learning Framework for Intelligent Plant Disease Detection. GitHub Repository.
