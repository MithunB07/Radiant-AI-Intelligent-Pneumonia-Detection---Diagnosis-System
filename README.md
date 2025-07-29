# Radiant-AI: Intelligent Pneumonia Detection & Diagnosis System 🧠🫁

A deep learning–powered web application built with **Flask**, designed to **detect pneumonia** from chest X-ray images with high accuracy and intuitive visual explanations.

---

## 🚀 Project Overview

Radiant-AI enables users to upload chest X-rays and get immediate predictions on whether the image indicates **Pneumonia** or **Normal (No Pneumonia)**. It uses a **custom CNN model inspired by ResNet**, trained on publicly available Kaggle datasets.

Key highlights:

- Upload image → Predict → Visualize heatmap.
- Provides **confidence score** and **three-level Grad-CAM heatmaps**:
  - 🔴 **Red** – Highly affected
  - 🟠 **Orange** – Moderately affected
  - 🟡 **Yellow** – Mild or negligible signs

---

## 🧠 Model Details

- **Architecture**: Custom CNN based on ResNet principles
- **Training**: Done from scratch using Kaggle Chest X-ray Pneumonia dataset
- **Accuracy**: Achieved **~97%** accuracy on validation data
- **Deployment**: Trained in **Google Colab**, saved, and used for real-time prediction via Flask

---

## 🛠 Tech Stack

| Layer        | Technology               |
|--------------|---------------------------|
| Framework    | Flask (Python)            |
| Deep Learning| TensorFlow / Keras        |
| Visualization| Grad-CAM (heatmap overlay)|
| Frontend     | HTML + CSS (via templates)|

---

## 📂 Project Structure

```
Mini-Project/
├── app.py                  # Main Flask application
├── models/
│   └── trained_model_pneumonia.h5
├── static/
│   ├── uploaded images
│   └── Grad-CAM overlays (auto-generated)
├── templates/
│   ├── index.html
│   └── about.html, contact.html, etc.
├── requirements.txt
├── .gitignore
```

---

## 💻 Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/MithunB07/Radiant-AI-Intelligent-Pneumonia-Detection---Diagnosis-System.git
cd Radiant-AI-Intelligent-Pneumonia-Detection---Diagnosis-System
```

### 2. Create a virtual environment

```bash
python -m venv venv
venv\Scriptsctivate     # On Windows
# OR
source venv/bin/activate  # On macOS/Linux
```

### 3. Install the dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Flask app

```bash
python app.py
```

Then visit `http://127.0.0.1:5000` in your browser.

---

## 📸 Features

- Upload chest X-ray images
- Get prediction: **Pneumonia** or **Normal**
- View **confidence score**
- Visualize affected areas using **Grad-CAM**
  - Shows high/medium/low impact regions in color overlay

---

## 🔬 Dataset

- **Source**: Kaggle Chest X-ray Pneumonia Dataset
- **Categories**:
  - Normal
  - Pneumonia (Bacterial/Viral not separated in prediction)

---

## 📊 Results

| Metric   | Score     |
|----------|-----------|
| Accuracy | 97%       |
| Confidence | Per Image |

*(Note: Full evaluation report and metrics will be added soon)*

---

## 🔒 Limitations

- Trained only for binary classification: **Pneumonia** vs. **No Pneumonia**
- Not deployed to cloud yet
- Should not be used as a clinical tool without further validation

---

## 📽️ Demo

*A demo video and screenshots will be added soon.*

---

## 🤝 Contributing

Want to improve this project? Here’s how:

1. Fork the repo
2. Create a new branch (`feature/my-update`)
3. Commit your changes
4. Push to your branch
5. Submit a Pull Request

---

## 👨‍💻 Authors

- **[Jayashri Krishnan]**
- **[Mithun B ]** 
- **[Kiran Kumar AJ]**
- **[Dharini S]**

---

## 📄 License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgements

- [Kaggle Chest X-ray Pneumonia Dataset](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia)
- [Grad-CAM Paper](https://arxiv.org/abs/1610.02391)
- Google Colab for training infrastructure