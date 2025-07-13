# 🐶🐱 Task 3 – Cats vs Dogs Image Classification using SVM

As part of my internship at **SkillCraft Technology**, I implemented a basic **Support Vector Machine (SVM)** model to classify images of cats and dogs based on pixel-level features.

---

## 🎯 Objective

To build a supervised image classification model that:
- 📦 Reads images of cats and dogs
- 🧠 Trains an SVM classifier on raw pixel values
- 🖼 Predicts whether an image is a cat 🐱 or a dog 🐶

---

## 🗂 Dataset

- **Name:** Kaggle Dogs vs Cats (subset)
- **Images Used:** 1000 cats + 1000 dogs = 2000 total
- **Image Size:** 64×64 resized RGB images

---

## ⚙️ Technologies Used

- Python
- OpenCV
- NumPy
- scikit-learn
- Matplotlib

---

## 🔁 Workflow

1. **Unzipped** `dogs-vs-cats.zip`
2. **Loaded & Resized** each image to 64x64
3. **Flattened** images to 1D vectors for SVM input
4. **Split** data (80% training, 20% testing)
5. **Trained** an SVM classifier (`linear` kernel)
6. **Evaluated** performance using accuracy & classification report
7. **Visualized** predictions with sample images

---

## ✅ Results

- **Total Images Used:** 2000  
- **Test Set Accuracy:** **57%**
- **Classification Report:**

| Class | Precision | Recall | F1-score |
|-------|-----------|--------|----------|
| Dog   | 0.58      | 0.47   | 0.52     |
| Cat   | 0.56      | 0.67   | 0.61     |

⚠️ This basic approach uses **raw pixel values** — performance is limited. Future improvements may include using:
- CNNs (Convolutional Neural Networks)
- Feature extraction (HOG, deep features)
- Image augmentation

---

## 📸 Sample Output (Prediction)

```plaintext
Image: 🐶
Predicted: Dog | Actual: Dog

Image: 🐱
Predicted: Cat | Actual: Cat
