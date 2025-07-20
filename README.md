#  Glaucoma Detection Using Deep Learning - Desai Eye Hospital Project

>  Accepted for **Oral Presentation** at the **9th IEEE International Conference**

---

##  Project Overview

This project focuses on the **automated detection of Glaucoma** from retinal fundus images using **transfer learning with VGG16**. It was developed as a collaboration with **Desai Eye Hospital** to assist doctors in early diagnosis and improve accessibility for rural patients.

---

##  Technologies Used

- Python
- TensorFlow / Keras
- OpenCV
- VGG16 (Transfer Learning)
- Matplotlib, Seaborn
- scikit-learn

---

##  Dataset

- Total images: **150**
  - 120 images of *Glaucoma*
  - 30 images of *Normal*
- Balanced Dataset used: **30 Glaucoma + 30 Normal**
- Folder structure:desia_eye/
├── glaucoma/
└── normal/


---

##  Preprocessing Steps

- Image resizing to **224×224×3** (for VGG16)
- Normalization (pixel values scaled 0–1)
- Label encoding: `Glaucoma = 0`, `Normal = 1`
- Balanced subset selection to avoid class imbalance
- Visual comparison of original and resized images

---

##  Model: VGG16 (Transfer Learning)

- Pretrained **VGG16** model without top layers
- Custom classifier added with:
- Flatten
- Dense (ReLU, 128)
- Dropout (0.5)
- Final Dense with Sigmoid (binary classification)
- Trainable params limited to the top classifier only

---

##  Results

| Metric       | Value     |
|--------------|-----------|
| Accuracy     | 91.67%    |
| Loss         | 0.32      |
| Model Type   | Binary CNN (VGG16) |
| Image Input  | 224x224 RGB |
| Framework    | TensorFlow/Keras |

---

## 🖼 Visualization

- Training vs Validation Accuracy
- Confusion Matrix
- Before vs After Preprocessing
- Misclassified image review

---

##  Real-World Use Case

- Designed for **Desai Eye Hospital** to assist in early screening of glaucoma.
- Can be integrated into:
- Doctor dashboard
- Mobile notification system for patients
- AI-powered chatbot for rural outreach

---

##  Conference Recognition

>  This project has been **accepted for Oral Presentation** at the **IEEE 9th International Conference** for its innovation in AI-based medical diagnosis.

---



