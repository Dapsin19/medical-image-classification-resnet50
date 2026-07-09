# 🩺 Medical Image Classification using ResNet50 & FastAPI

An AI-powered medical image classification system built with **PyTorch**, **ResNet50**, and **FastAPI**. The application classifies chest X-ray images as **Normal** or **Pneumonia** using transfer learning and exposes a production-ready REST API for inference.

---

## Project Overview

This project demonstrates how deep learning models can support medical image analysis by automatically detecting pneumonia from chest X-ray images.

The model is based on **ResNet50** pretrained on ImageNet and fine-tuned for binary chest X-ray classification.

The trained model is deployed through a **FastAPI REST API**, allowing users to upload X-ray images and receive predictions with confidence scores.

---

## Features

- Transfer Learning using ResNet50
- Chest X-ray image classification
- Confidence score for every prediction
- FastAPI REST API
- Image preprocessing pipeline
- Production-ready project structure
- Automated API testing with PyTest

---

## Dataset

Dataset:

**Chest X-Ray Images (Pneumonia)**

Source:
https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia

Classes:

- NORMAL
- PNEUMONIA

---

## Tech Stack

- Python
- PyTorch
- Torchvision
- ResNet50
- FastAPI
- Pillow
- NumPy
- PyTest

---

## Project Structure

```
medical-image-classification-resnet50/

├── app.py
├── model.py
├── medical_model.pth
├── requirements.txt
├── README.md
├── LICENSE
├── .gitignore

└── test_api.py
```

---

## Installation

Clone the repository

```bash
git clone https://github.com/Dapsin19/medical-image-classification-resnet50.git
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the API

```bash
uvicorn app:app --reload
```

The API will be available at

```
http://127.0.0.1:8000/docs
```

---

## API Usage

### POST `/predict`

Upload a chest X-ray image.

Example Response

```json
{
    "prediction": "PNEUMONIA",
    "confidence": 0.9824
}
```

---



## Future Improvements

- Docker deployment
- Multi-class disease classification
- Grad-CAM visual explanations
- Cloud deployment (AWS/Azure/GCP)
- Model monitoring
- CI/CD pipeline

---

## Skills Demonstrated

- Deep Learning
- Computer Vision
- Transfer Learning
- Medical Image Classification
- REST API Development
- Model Deployment
- PyTorch
- FastAPI

---

## License

MIT License
