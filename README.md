# 🐶🐱 CNN ile Kedi vs Köpek Görüntü Sınıflandırma  

### 🔗 Kaggle Notebook Linki: https://www.kaggle.com/code/ozlemlimon/dogs-vs-cats-cnn-image-classification


## 📌 Projenin Amacı  
Bu proje, **Convolutional Neural Network (CNN)** kullanarak **kedi** ve **köpek** resimlerini sınıflandırmayı amaçlayan bir derin öğrenme çalışmasıdır.  
Amaç, temel CNN yapısını öğrenmek, veri artırma (data augmentation), hiperparametre optimizasyonu ve model performans değerlendirme adımlarını uygulamaktır.  

---

## 📂 Dataset Bilgisi  
- Dataset: [Dogs vs Cats (Kaggle)](https://www.kaggle.com/competitions/dogs-vs-cats/data)  
- Kategoriler:  
  - **Cat (Kedi)**  
  - **Dog (Köpek)**  
- Dataset `train`, `validation`, `test` olarak üçe ayrılmıştır.  
- Görseller **128x128 piksel** boyutuna dönüştürülmüştür.  

---

## 🛠️ Kullanılan Yöntemler  

### 1. Veri Ön İşleme & Data Augmentation  
- Görsellerin yeniden boyutlandırılması  
- Eğitim / validation / test ayrımı  
- Data Augmentation:  
  - Random Flip  
  - Random Rotation  
  - Random Zoom  

### 2. CNN Model Mimarisi  
- Convolutional Layers  
- Batch Normalization  
- MaxPooling  
- Dropout  
- Dense Layers + Softmax çıkış  

### 3. Eğitim ve Callbacks  
- **Epochs:** 25  
- **Callbacks:**  
  - EarlyStopping  
  - ModelCheckpoint  
  - ReduceLROnPlateau  
  - TensorBoard  

### 4. Model Değerlendirme  
- Accuracy & Loss grafiklerinin analizi  
- Confusion Matrix & Classification Report  
- ROC Curve ve AUC  
- Precision, Recall, F1 skorlarının görselleştirilmesi  

### 5. Model Açıklanabilirliği  
- **Grad-CAM** yöntemi ile modelin tahmin sırasında dikkate aldığı bölgelerin görselleştirilmesi  

### 6. Hiperparametre Optimizasyonu  
- **Keras Tuner** ile:  
  - Filtre sayısı  
  - Katman sayısı  
  - Dropout oranı  
  - Dense layer boyutu  
  - Learning rate  

---

## 📊 Sonuçlar  
- Model, test setinde başarılı bir doğruluk oranı elde etmiştir.  
- Data augmentation ve dropout sayesinde **overfitting azaltılmıştır**.  
- ROC ve AUC analizleri, modelin güvenilir bir sınıflandırma performansı sunduğunu göstermektedir.  
- Grad-CAM görselleştirmeleri, modelin genellikle hayvanların **yüz bölgesine odaklandığını** ortaya koymaktadır.  

---

## 💾 Modelin Kaydedilmesi  
En iyi model `.h5` formatında kaydedilmiştir ve tekrar kullanılabilir.  

```bash
dogs_vs_cats_best_model.h5


