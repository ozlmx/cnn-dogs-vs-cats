
# CNN ile Kedi-Köpek Sınıflandırma Projesi

Bu repo, **Global AI Hub Bootcamp** kapsamında geliştirdiğim ilk **CNN tabanlı derin öğrenme projesini** içermektedir.  
Amaç, **Cats vs Dogs** veri seti kullanılarak bir görüntü sınıflandırma modeli oluşturmak ve sonuçlarını değerlendirmektir.  

---

## 📌 Giriş

Bu projede kullanılan veri seti, Kaggle üzerinde bulunan **Dogs vs Cats** veri setidir.  
- Veri setinde iki sınıf bulunmaktadır: **Cat** ve **Dog**.  
- Görseller eğitim ve test olmak üzere ayrılmıştır.  
- Kullanılan model, **Convolutional Neural Network (CNN)** mimarisine dayanmaktadır.  

Model, sıfırdan CNN katmanları ile kurulmuş olup, aşağıdaki adımlar uygulanmıştır:  
1. Veri yükleme ve ön işleme  
2. CNN mimarisinin oluşturulması  
3. Modelin eğitilmesi  
4. Başarı metriklerinin hesaplanması  
5. Sonuçların yorumlanması  

---

## ⚙️ Teknik Detaylar

- **Derin Öğrenme Frameworkü:** TensorFlow / Keras  
- **Model Tipi:** Convolutional Neural Network (CNN)  
- **Kullanılan Katmanlar:** Conv2D, MaxPooling2D, Flatten, Dense, Dropout  
- **Optimizer:** Adam  
- **Loss Function:** Binary Crossentropy  
- **Metric:** Accuracy  

---

## 📊 Metrikler

Modelin eğitimi sonucunda elde edilen performans metrikleri aşağıda verilmiştir:

### Test Sonuçları
- **Toplam Test Örneği:** 12.461  
- **Accuracy:** %65  
- **Macro Avg (Precision / Recall / F1):** %65 / %65 / %65  
- **Weighted Avg (Precision / Recall / F1):** %65 / %65 / %65  

### Sınıf Bazlı Performans
| Sınıf | Precision | Recall | F1-Score | Destek (Support) |
|-------|-----------|--------|----------|------------------|
| Cat   | 0.65      | 0.65   | 0.65     | 6242             |
| Dog   | 0.65      | 0.65   | 0.65     | 6219             |

---

## 🔎 Sonuç ve Yorum

- Model, **her iki sınıfta da dengeli bir başarı** göstermektedir.  
- Precision, Recall ve F1-score değerleri %65 seviyesinde olup, **orta düzey bir doğruluk** elde edilmiştir.  
- Sınıflar arasında belirgin bir dengesizlik gözlenmemiştir.  

---

## 🚀 Gelecek Çalışmalar

Modelin performansını artırmak için yapılabilecek geliştirmeler:  
- **Data Augmentation:** Görselleri çeşitlendirmek için döndürme, kırpma, zoom, parlaklık ayarı vb. yöntemler eklenebilir.  
- **Transfer Learning:** Daha güçlü önceden eğitilmiş modeller (VGG16, ResNet, Inception) kullanılabilir.  
- **Hiperparametre Optimizasyonu:** Learning rate, batch size ve epoch sayısı üzerinde iyileştirmeler yapılabilir.  
- **Deployment:** Model, bir web arayüzü (ör. Streamlit) ile entegre edilerek son kullanıcıya sunulabilir.  


## Linkler:
### 🔗 Kaggle Notebook Linki: https://www.kaggle.com/code/ozlemlimon/dogs-vs-cats-cnn-image-classification
### 🔗 Kullanılan Kaggle Dataset Linki: https://www.kaggle.com/datasets/moazeldsokyx/dogs-vs-cats




