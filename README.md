# cats-vs-dogs-classificaiton-project

## Giriş
Bu projede, **Microsoft Cats vs Dogs** veri seti kullanılarak bir **ikili sınıflandırma (binary classification)** modeli geliştirilmiştir.  
Amaç, verilen bir görselin **kedi mi yoksa köpek mi** olduğunu doğru şekilde tahmin etmektir.  

Projede:
- **CNN tabanlı bir derin öğrenme modeli** uygulanmıştır.
- Görseller **ImageDataGenerator** ile yeniden ölçeklendirilmiş ve eğitim/doğrulama için ayrılmıştır.
- Model, farklı hiperparametre ayarları ile test edilmiştir.
- Eğitim sürecinde doğruluk ve kayıp grafikleri incelenmiş, ek olarak confusion matrix ve classification report ile değerlendirme yapılmıştır.

Notebook içerisinde hem kodlar hem de **markdown hücreleriyle teknik açıklamalar** eklenmiştir.  

## Metrikler
Modelin değerlendirmesinde kullanılan metrikler:  
- **Accuracy (Doğruluk)**
- **Loss (Kayıp)**
- **Confusion Matrix**
- **Classification Report (Precision, Recall, F1-score)**  

Sonuçlara göre:  
- Eğitim ve doğrulama setlerinde tutarlı bir başarı elde edilmiştir.  
- Farklı optimizasyon algoritmaları (ör. `Adam`, `RMSprop`) ve learning rate denemeleri yapılmıştır.  
- Hiperparametre denemeleri sonucunda en iyi doğrulama başarısı Adam optimizeri ile %80.62 seviyelerine ulaşmıştır.  
- Confusion Matrix ile hataların hangi sınıflarda yoğunlaştığı gözlemlenmiştir.  

Bu sonuçlar, modelin kedi ve köpek görsellerini ayırt etmede **başarılı bir temel model** olduğunu göstermektedir. 



## Ekler
Bu projede şu anda temel eğitim ve değerlendirme adımları gerçekleştirilmiştir.  
Henüz bir **deployment (Streamlit, Flask vb.)** yapılmamıştır.  



## Sonuç ve Gelecek Çalışmalar
Bu proje, benim için **CNN tabanlı image classification** konusunda bir başlangıç niteliği taşımaktadır.
Bu nedenle bazı kodları yazarken ve fikirleri geliştirirken AI araçlarından destek aldım. Bu süreç, öğrenme ve geliştirme deneyimime katkı sağladı; tüm kodları ve hiperparametre seçimlerini kendim anlayarak uyguladım.
Bazı aşamalarda özellikle Grad-CAM ve Eigen-CAM görselleştirmeleri teknik kısıtlamalar ve veri dosyalarındaki sorunlar nedeniyle tamamlanamadı. Ancak modelin eğitimi, hiperparametre optimizasyonu ve doğrulama süreçleri tamamlandı.

Gelecekte modeli geliştirmek için: 
- Heatmap görselleştirmeleri eklenebilir. 
- Modelin doğruluğu artırılabilir.
- Daha büyük ve dengeli veri setleri kullanılabilir.  
- Kullanıcı dostu bir arayüzü ile deploy edilebilir.
- Modelin kaydedilmesi ve yüklenmesi (`model.save()` & `load_model`) yapılabilir. 
- Veri artırma (data augmentation) yöntemleri çeşitlendirilebilir.  
- Gerçek zamanlı veri ile güncellemeler yapılabilir.
- Transfer Learning (örn. VGG16, ResNet) ile daha güçlü sonuçlar alınabilir.  

 

## Linkler
https://www.kaggle.com/code/nisanurkk/cats-vs-dogs-classificaiton-project
