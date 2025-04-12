# SpotTheBot

This project aims to classify whether an image is **real** or **AI-generated**, using two state-of-the-art deep learning models: **EfficientNet-B3** and **Swin Transformer**. It's wrapped in a professional and user-friendly **Streamlit app** that includes image upload, prediction, and Grad-CAM-based visual explanation.

---

##  Key Features

-  Classifies images as **Real** or **Fake**
-  Built using **EfficientNet-B3** and **Swin Transformer**
-  Real-time predictions via a **Streamlit web app**
-  Visual explainability using **Grad-CAM**
-  Analysis of model weaknesses on stylized art

---

##  Models Used

###  EfficientNet-B3
- Pretrained on ImageNet
- Custom classifier head
- Selective fine-tuning of top convolution blocks
- Grad-CAM integrated for interpretability

###  Swin Transformer
- Hierarchical Vision Transformer (via `timm`)
- Transformer layers frozen initially
- Classification head retrained

---

##  Dataset Overview

- **Real Images**: Natural photos from open datasets
- **Fake Images**: AI-generated from models like Midjourney, DALL·E, etc.
- Transforms:
  - Resize to 224×224
  - Normalize using ImageNet mean & std

---

## ⚙️ How to Run

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/fake-image-detector.git
cd fake-image-detector```
```streamlit run app.py```

