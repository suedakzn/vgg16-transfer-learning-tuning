# vgg16-transfer-learning-tuning

##  CNN Image Classification with VGG16 & Hyperparameter Tuning

Bu projede **Convolutional Neural Network (CNN)** tabanlı bir görüntü sınıflandırma modeli geliştirdim.  
Amacım sıfırdan bir CNN kurmak, ardından **transfer learning (VGG16)** ve **fine-tuning** ile performansı artırmak, sonrasında da **hiperparametre optimizasyonu (Keras Tuner)** ile farklı kombinasyonları deneyip sonuçları kıyaslamaktı.   Ayrıca **Eigen-CAM** yöntemiyle modelin görsellere nasıl odaklandığını görselleştirdim.   

---

## Proje Akışı
1. **Veri Önişleme & Manipülasyon**
   - ImageDataGenerator ile veri artırma (rotation, shift, zoom, flip, normalization).  
   - Train/validation/test ayrımı.  

2. **Modelleme**
   - **İlk CNN Modelim**: Basit bir CNN kurdum, temel doğruluk değerlerini inceledim.  
   - **Transfer Learning (VGG16)**: Önceden eğitilmiş VGG16 ile %90 doğruluk elde ettim.  
   - **Fine-Tuning**: VGG16’nın son bloklarını açarak daha iyi genelleme sağladım.  
   - **Hyperparameter Optimization**: Katman sayısı, filtre, kernel, dropout, dense units, learning rate ve optimizer parametrelerinde arama yaptım.  

3. **Değerlendirme**
   - Accuracy & Loss grafiklerini çizdim.  
   - Test setinde classification report ve confusion matrix ile sınıflar bazında performansı analiz ettim.  
   - Eigen-CAM ile modelin odaklandığı bölgeleri görselleştirdim.  

---

## Kullanılan Teknolojiler
- Python 
- TensorFlow / Keras  
- Keras Tuner  
- Scikit-learn  
- Matplotlib, Seaborn  
- OpenCV  

---

## Sonuçlar
- **Transfer Learning (VGG16)**: Doğruluk ~%90  
- **Fine-Tuning**: Daha stabil ve yüksek genelleme başarımı  
- **Hyperparameter Tuning**: Farklı kombinasyonlar denendi ama transfer learning daha güçlü sonuç verdi  
- **Test Sonucu**: ~%79–91 arası doğruluk (modele göre değişti)  
- **En büyük karışma**: Glacier ↔ Mountain sınıflarında  
- **En iyi sınıf**: Forest (neredeyse kusursuz tahmin)  

---

## Gelecek Çalışmalar
- Daha büyük/dengeli veri seti ile performans artırma  
- EfficientNet, ResNet gibi farklı pre-trained modeller deneme  
- Daha gelişmiş optimizasyon yöntemleri (Bayesian Optimization, Hyperband)  
- Gerçek uygulama entegrasyonu (mobil/web deployment)  

---

## 📌 Not
Bu proje, derin öğrenme alanında **CNN mimarisi, transfer learning, fine-tuning, hyperparameter tuning ve model görselleştirme** konularında deneyim kazanmak için yapılmıştır.
