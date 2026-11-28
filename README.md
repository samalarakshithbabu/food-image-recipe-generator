# 🍔 Food Image Recipe Generator

<div align="center">

![Python](https://img.shields.io/badge/python-3.8%2B-blue?logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-3.0-black?logo=flask)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.15-orange?logo=tensorflow)
![VGG16](https://img.shields.io/badge/VGG16-DeepLearning-red)
![Groq](https://img.shields.io/badge/Groq-LLaMA-blue)

**AI-Powered Food Recognition & Nutrition Generator**

[![View Demo](https://img.shields.io/badge/View-Demo-blue)]()
[![Report Issue](https://img.shields.io/badge/Report-Issue-red)](https://github.com/samalarakshithbabu/food-image-recipe-generator/issues)

</div>

---

## 🚀 Executive Summary

An **AI-powered web application** that identifies food from images and generates instant ingredient lists and nutrition facts using deep learning (VGG16) and the Groq LLM (LLaMA 3.3). Just snap a photo and learn what's on your plate!

### What It Does

```mermaid
graph LR
    A[Food Image] --> B[VGG16 Model]
    B --> C[101 Food Categories]
    C --> D[Groq LLM API]
    D --> E[Ingredients & Nutrition]
    E --> F[Dashboard Display]
```

---

## ✨ Key Features

| Feature | Description |
|---------|-------------|
| **Food Recognition** | Classifies from 101 food categories |
| **VGG16 Deep Learning** | Custom-trained CNN model |
| **Smart Ingredient Generation** | Groq LLM (LLaMA 3.3 70B) |
| **Nutrition Facts** | AI-generated nutritional information |
| **Modern UI** | Responsive HTML + Tailwind CSS |

---

## 🧠 Model Details

| Aspect | Details |
|--------|---------|
| **Architecture** | VGG16 (no top layers) |
| **Dataset** | Food-101 with augmentations |
| **Classes** | 101 food categories |
| **Training** | ~80 epochs, batch size 16 |

---

## 🛠️ Technology Stack

| Component | Technology | Purpose |
|-----------|------------|---------|
| **Backend** | Python + Flask | Web server |
| **Deep Learning** | TensorFlow/Keras | VGG16 model |
| **LLM** | Groq API | Ingredient generation |
| **Frontend** | HTML + TailwindCSS | UI |

---

## 📁 Project Structure

```
food-image-recipe-generator/
├── app.py                          # Flask backend
├── model.py                        # Model architecture & training
├── vgg16_food101_trained.h5       # Trained model weights
├── templates/
│   └── index.html                  # Dashboard UI
├── static/                         # Styles/images
├── api.txt                         # API key & labels
└── README.md                       # This file
```

---

## 🛠️ Installation

### Prerequisites
- Python 3.8+
- Groq API key

### Setup
```bash
git clone https://github.com/samalarakshithbabu/food-image-recipe-generator.git
cd food-image-recipe-generator
pip install -r requirements.txt

# Set Groq API key in api.txt or environment
python app.py
```

---

## ⚠️ Limitations

| Limitation | Description |
|------------|-------------|
| **Model File** | vgg16_food101_trained.h5 may be large |
| **API Key Required** | Groq API key needed for nutrition |
| **Accuracy** | Claims not independently verified |

---

## 📄 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**SAMALA RAKSHITH BABU**

- 📧 Email: samalarakshithbabu7@gmail.com
- 💼 LinkedIn: [samala-rakshith-babu](https://www.linkedin.com/in/samala-rakshith-babu/)
- 🐙 GitHub: [samalarakshithbabu](https://github.com/samalarakshithbabu)