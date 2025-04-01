# 📚 Student Exam Performance Prediction

![Machine Learning](https://miro.medium.com/max/1400/1*5ZbDmzZATvEYvlAUft6Ukw.png)

This project is an end-to-end Machine Learning application that predicts students' exam scores based on various features. It follows a structured ML pipeline and is built using Flask for deployment.

---

## 🚀 Features

- **End-to-End ML Pipeline**: Data ingestion, preprocessing, model training, evaluation, and prediction.
- **Flask API**: Interactive UI for users to input student data and get predictions.
- **Model Persistence**: Uses pickle to store and load trained models.
- **Exception Handling**: Custom exception handling for better debugging.
- **Modular Codebase**: Organized structure for easy scalability and maintainability.

---

## 🛠 Tech Stack

- **Python** (pandas, numpy, sklearn, pickle)
- **Flask** (for API deployment)
- **HTML/CSS** (for UI)
- **AWS Elastic Beanstalk** (for deployment - optional)

---

## 📂 Project Structure

```
END_TO_END_ML_PROJECT/
│── artifacts/                  # Stores processed data & trained models
│── src/
│   ├── components/             # Data ingestion, transformation, model trainer
│   ├── pipeline/               # Training & Prediction pipeline
│   ├── exception.py            # Custom exception handling
│   ├── logger.py               # Logs for debugging
│   ├── utils.py                # Utility functions (save, load, etc.)
│── app.py                      # Flask application
│── templates/
│   ├── home.html               # Main page UI
│── requirements.txt            # Dependencies
│── README.md                   # Project documentation
```

---

## 🔧 Installation & Setup

1️⃣ **Clone the Repository**
```bash
git clone https://github.com/SubhashGovindharaj/end_to_end_ml_project.git
cd end_to_end_ml_project
```

2️⃣ **Create Virtual Environment & Install Dependencies**
```bash
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

3️⃣ **Run the Flask App**
```bash
python app.py
```
Access the app at: **http://127.0.0.1:5000/**

---

## 🔥 Model Training & Prediction

🔹 **Train the Model**
```bash
python src/pipeline/train_pipeline.py
```
🔹 **Make Predictions**
```bash
python src/pipeline/predict_pipeline.py
```

---

## 🚀 Deployment (Optional)

### 📌 Deploy on AWS Elastic Beanstalk

1️⃣ Install AWS CLI & Elastic Beanstalk CLI
```bash
pip install awsebcli --upgrade --user
```

2️⃣ Initialize & Deploy
```bash
eb init -p python-3.8 student-performance-app --region us-east-1
eb create student-predict-env
```

3️⃣ Open the Deployed App
```bash
eb open
```

---

## 📸 Screenshots

### 🎯 Home Page
![Home Page](https://user-images.githubusercontent.com/your-image-link.png)

### 🎯 Prediction Result
![Prediction Result](https://user-images.githubusercontent.com/your-image-link.png)

---

## 👨‍💻 Author

**Subhash Govindharaj**

📧 Email: [subhashgovidharaj@gmail.com](mailto:subhashgovindharaj@gmail.com)  
🔗 GitHub: [SubhashGovindharaj](https://github.com/SubhashGovindharaj)  

---

## ⭐ If you like this project, give it a star! ⭐
