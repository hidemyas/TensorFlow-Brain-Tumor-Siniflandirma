# TensorFlow ile Beyin Tümörü MRI Sınıflandırması

---

## Projenin Amacı
Bu projenin amacı, MRI görüntüleri kullanılarak beyin tümörlerinin sınıflandırılması için bir **derin öğrenme modeli** geliştirmektir. Proje, görüntü analizinde otomatik teşhisin bir yardımcı araç olarak potansiyelini göstermektedir.

## Veri Seti Hakkında Bilgi
Bu projede kullanılan veri seti, **Kaggle Brain Tumor MRI Dataset**'idir. Veri seti, dört farklı beyin durumu için MRI görüntüleri içermektedir:
* Glioma
* Meningioma
* Notumor (Tümörsüz)
* Pituitary

## Kullanılan Yöntemler
Model, **VGG16** tabanlı bir **Evrişimsel Sinir Ağı (CNN)** mimarisi kullanılarak oluşturulmuştur. Proje kapsamında uygulanan başlıca adımlar şunlardır:
* **Veri Önişleme ve Artırma (Data Augmentation):** Modelin genelleme yeteneğini artırmak için veri artırma teknikleri kullanılmıştır.
* **Model Eğitimi:** Model, eğitim veri seti üzerinde eğitilerek tümör türlerini ayırt etmeyi öğrenmiştir.
* **Model Değerlendirmesi:** Modelin performansı, karmaşıklık matrisi (Confusion Matrix) ve sınıflandırma raporu (Classification Report) gibi metriklerle değerlendirilmiştir.
* **Grad-CAM Görselleştirme:** Modelin kararlarının yorumlanabilmesi için Grad-CAM tekniği ile görselleştirmeler yapılmıştır.

## Elde Edilen Sonuçlar
Proje kapsamında eğitilen model, test verileri üzerinde **%84 doğruluk** oranına ulaşmıştır. Elde edilen sınıflandırma raporu ve karmaşıklık matrisi, modelin her bir sınıf için ne kadar başarılı olduğunu göstermektedir.

