# svmMobileNet  

### Image Classification using MobileNetV2 + SVM  

This project implements an image classification model that combines **MobileNetV2** as a feature extractor and **Support Vector Machine (SVM)** as a classifier.  
It was applied on a **tomato image dataset** to distinguish between different categories (healthy vs. diseased).  

---

### Model Overview  
- **Feature extractor:** MobileNetV2 (pretrained on ImageNet)  
- **Classifier:** SVM (`sklearn.svm.SVC`)  
- **Frameworks:** TensorFlow, Scikit-learn, NumPy, Matplotlib  
- **Goal:** Achieve high accuracy while keeping the model lightweight and fast.  

---

###  Steps in the Notebook  
1. Load and preprocess images using TensorFlow’s `ImageDataGenerator`.  
2. Extract features with pretrained MobileNetV2 (without top layers).  
3. Train an SVM classifier on the extracted features.  
4. Evaluate model performance with metrics such as accuracy, F1-score, and confusion matrix.  

---

###  Results  
| Metric | Value (approx.) |
|---------|-----------------|
| Accuracy | 90–98% |
| Model Type | MobileNetV2 + SVM |

---

###   Requirements  
```bash
tensorflow>=2.8
scikit-learn
numpy
matplotlib

---

###   How to Run

git clone https://github.com/tari-hiba/svmMobileNet.git
cd svmMobileNet
jupyter notebook svmMobileNet.ipynb
