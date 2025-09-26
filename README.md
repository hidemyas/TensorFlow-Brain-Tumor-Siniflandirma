

# Akbank Derin Öğrenme Bootcamp Proje Repository

## Giriş

Bu repository, Akbank Derin Öğrenme Bootcamp kapsamında geliştirilen beyin tümörü MRI sınıflandırma projesini içermektedir. Proje, tıbbi görüntü işleme ve derin öğrenme tekniklerini kullanarak beyin tümörü türlerini (glioma, meningioma, no tumor, pituitary) sınıflandırmayı amaçlamaktadır.

Proje kapsamında:
- **Veri Seti**: Brain Tumor MRI Dataset (Kaggle)
- **Algoritmalar**: VGG16 tabanlı transfer öğrenme, CNN, Grad-CAM
- **Teknikler**: Veri artırma (data augmentation), hiperparametre optimizasyonu, model değerlendirme metrikleri

Projenin teknik detayları, notebook dosyası içinde markdown hemde yorum formatında açıklanmıştır.

## Metrikler

Model performansı aşağıdaki metriklerle değerlendirilmiştir:

- **Test Doğruluğu**: %94
- **Kayıp (Loss)**: 0.18
- **Sınıflandırma Raporu**: Her sınıf için precision, recall ve f1-score değerleri
- **Karmaşıklık Matrisi**: Modelin doğru ve yanlış sınıflandırmalarının dağılımı

Sonuçlar, modelin özellikle 'no tumor' ve 'pituitary' sınıflarında yüksek başarı elde ettiğini göstermektedir. 'Glioma' ve 'meningioma' sınıfları arasında bazı karışıklıklar gözlemlenmiştir, bu da bu iki tümör türünün benzer özellikler taşıdığını düşündürmektedir.

Grad-CAM görselleştirmesi, modelin sınıflandırma kararlarını verirken tümör bölgelerine odaklandığını doğrulamıştır. Bu, modelin tıbbi olarak anlamlı özellikleri öğrendiğini göstermektedir.

## Ekler

Proje kapsamında aşağıdaki ek çalışmalar gerçekleştirilmiştir:

- **Hiperparametre Optimizasyonu**: Farklı optimizer'lar (SGD, Adam), öğrenme oranları, dropout oranları ve batch size'lar karşılaştırılarak en iyi hiperparametreler belirlenmiştir.
- **GPU Optimizasyonu**: Model eğitimi sırasında GPU hızlandırma kullanılmıştır.
- **Deployment Hazırlığı**: Streamlit ile kullanıcı arayüzü oluşturmak için temel kod yapısı hazırlanmıştır (UI klasörü).

## Sonuç ve Gelecek Çalışmalar

Bu proje, tıbbi görüntü işleme alanında derin öğrenme tekniklerinin etkili bir şekilde kullanılabileceğini göstermiştir. Elde edilen %94'lük doğruluk oranı, modelin klinik uygulamalar için potansiyel taşıdığını göstermektedir.

Gelecek çalışmalar için şu geliştirmeler planlanmaktadır:

1. **Daha Geniş Veri Seti**: Farklı hastanelerden ve tarama cihazlarından elde edilmiş daha çeşitli MRI görüntüleri eklenerek modelin genelleme yeteneği artırılabilir.
2. **Gerçek Zamanlı Sınıflandırma**: Modelin web kamerası veya doğrudan MRI cihazlarından gelen görüntüleri gerçek zamanlı olarak sınıflandırabilmesi için bir sistem geliştirilebilir.
3. **3D MRI İşleme**: Mevcut 2D MRI görüntüleri yerine 3D MRI verileri üzerinde çalışan bir model geliştirilerek daha kapsamlı analiz yapılabilir.
4. **Klinik Entegrasyon**: Modelin hastane bilgi sistemlerine entegre edilerek doktorların karar destek sistemi olarak kullanılması sağlanabilir.
5. **Mobil Uygulama**: Hasta ve doktorların mobil cihazlar üzerinden MRI görüntülerini yükleyerek ön teşhis alabilecekleri bir uygulama geliştirilebilir.

## Linkler

Projenin Kaggle üzerindeki notebook'una aşağıdaki linklerden erişebilirsiniz:
https://www.kaggle.com/code/hidemyas/tensorflow-ile-brain-tumor-mri-s-n-fland-rmas
- [Brain Tumor MRI Classification with TensorFlow]([https://www.kaggle.com/code/username/brain-tumor-mri-classification](http://kaggle.com/code/hidemyas/tensorflow-ile-brain-tumor-mri-s-n-fland-rmas/notebook))
- [Dataset]([https://www.kaggle.com/code/username/brain-tumor-gradcam-visualization](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset))

---

*Bu repository, Akbank Derin Öğrenme Bootcamp projesi kapsamında oluşturulmuştur.*


