# Food Image Recipe Generator

An intelligent web-based dashboard that recognizes food from images and generates instant ingredient lists and nutrition facts using deep learning and large language models.

---

## Problem Statement

Manual food identification and nutrition lookup is tedious. This system automates food recognition from images and provides AI-generated ingredient and nutrition information.

## Objectives

- Classify food images into 101 categories using VGG16
- Generate ingredient lists and nutrition facts via LLM
- Provide a responsive web interface for image upload
- Display predictions and nutritional information side-by-side

## Key Features

- **Food Image Recognition** — upload a photo; AI classifies from 101 food categories
- **Deep Learning Model** — custom-trained VGG16 CNN architecture
- **Smart Ingredient & Nutrition Generation** — Groq LLM API (LLaMA 3.3 70B) for human-readable insights
- **Modern UI** — responsive HTML + TailwindCSS frontend
- **Interactive Output** — predictions, ingredients, and nutritional content displayed together

## How It Works

1. **Frontend**: User uploads an image via dashboard UI
2. **Backend**:
   - Image is processed and resized (224×224)
   - Fed into trained VGG16 model (`vgg16_food101_trained.h5`)
   - Predicted class passed to Groq LLM to fetch ingredients and nutritional facts
3. **Results**: Displayed in real-time

## Model Details

- Based on VGG16 architecture (no top layers)
- Trained on Food-101 dataset with image augmentations
- 101 output classes (softmax layer)
- ~80 epochs, batch size 16

## Technologies Used

| Component | Technology |
|-----------|-----------|
| Backend | Python (Flask) |
| Deep Learning | TensorFlow/Keras (VGG16) |
| LLM | Groq API (LLaMA 3.3 70B) |
| Frontend | HTML, TailwindCSS |

## Project Structure

```
food-image-recipe-generator/
├── app.py                          # Flask backend for image upload and API
├── model.py                        # Model architecture and training code
├── vgg16_food101_trained.h5       # Trained model weights
├── templates/
│   └── index.html                  # Dashboard UI
├── static/                         # Optional styles/images
├── api.txt                         # API key and class labels
└── README.md
```

## Installation and Setup

### Prerequisites
- Python 3.8+
- pip
- Groq API key

### Setup
```bash
pip install -r requirements.txt
# Set Groq API key in api.txt or environment variable
python app.py
```

## Limitations

- Model file (`vgg16_food101_trained.h5`) is large and may not be included in repository
- Accuracy claims not independently verified
- Requires Groq API key for nutrition generation

## Author and Contact Information

**SAMALA RAKSHITH BABU**

- Email: samalarakshithbabu7@gmail.com
- LinkedIn: https://www.linkedin.com/in/samala-rakshith-babu-9374ab281/
- GitHub: https://github.com/samalarakshithbabu

## License

No LICENSE file present in repository.