# vgg16-transfer-learning-tuning

##  CNN Image Classification with VGG16 & Hyperparameter Tuning

Bu proje, **Convolutional Neural Network (CNN)** tabanlı bir görüntü sınıflandırma çalışmasıdır.  
Amacım, transfer learning (VGG16), fine-tuning, hiperparametre optimizasyonu (Keras Tuner) ve görselleştirme (Eigen-CAM) yöntemlerini kullanarak yüksek doğrulukta bir model geliştirmekti. 

##  Proje Hakkında
- İlk olarak sıfırdan kendi CNN modelimi kurdum ve temel sonuçları inceledim.  
- Daha sonra **VGG16 transfer learning** kullanarak performansı artırdım.  
- Son adımda **fine-tuning** ile VGG16’nın son bloklarını eğitime dahil ederek doğruluk oranını %90+ seviyelerine çıkardım.  
- **Keras Tuner** ile hiperparametre optimizasyonu yaparak modelin en iyi ayarlarını otomatik olarak seçtim.  
- **Eigen-CAM** ile modelin karar verirken odaklandığı bölgeleri görselleştirdim.

## Kullanılan Teknolojiler
- Python   
- TensorFlow / Keras  
- Keras Tuner  
- Matplotlib & Seaborn  
- OpenCV  
- Scikit-learn 
