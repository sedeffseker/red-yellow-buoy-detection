# İnsansız Deniz Aracı için Sarı ve Kırmızı Duba Tespiti

Bu proje, insansız deniz araçlarının (İDA) deniz ortamında
navigasyon amacıyla kullanılan sarı ve kırmızı dubaları
görüntü işleme ve yapay zekâ yöntemleri ile tespit edebilmesini
amaçlamaktadır.

---

## Veri Seti

Veri seti Roboflow platformu kullanılarak hazırlanmıştır.
Deniz ortamında çekilmiş sarı ve kırmızı dubalara ait görüntüler
toplanmış ve bounding box yöntemi ile elle etiketlenmiştir.

Veri seti eğitim, doğrulama ve test olmak üzere üçe ayrılmıştır.

---

## Ön İşleme (Preprocessing)

Model eğitimi öncesinde görüntüler yeniden boyutlandırılmış
ve normalize edilmiştir.
Bu adımlar, modelin daha kararlı ve hızlı öğrenebilmesi için
uygulanmıştır.

---

## Veri Artırma (Augmentation)

Bu projede veri artırma (augmentation) yöntemi kullanılmamıştır.
Mevcut veri seti, temel model eğitimi için yeterli görülmüştür.

---

## Model Seçimi

Bu projede nesne tespiti için YOLOv8 mimarisi kullanılmıştır.
YOLOv8, gerçek zamanlı çalışmaya uygun olması ve küçük nesnelerde
yüksek başarı göstermesi nedeniyle tercih edilmiştir.
Bu özellikleri sayesinde insansız deniz araçları gibi otonom
sistemler için uygundur.

---

## Model Eğitimi

Model eğitimi Python programlama dili kullanılarak gerçekleştirilmiştir.
Hazır YOLOv8 modeli, oluşturulan veri seti ile eğitilmiştir.
Eğitim süreci boyunca eğitim ve doğrulama verileri kullanılmıştır.

---

## Eğitim Sonuçları

Eğitim sürecinde modelin kayıp (loss) değerlerinde azalma,
doğruluk oranlarında ise artış gözlemlenmiştir.
Model, sarı ve kırmızı dubaları başarılı bir şekilde ayırt
edebilecek seviyeye ulaşmıştır.

---

## Kullanılan Kaynaklar

1. Object Detection for Maritime Navigation  
2. Buoy Detection Using Deep Learning  
3. YOLO-Based Maritime Object Detection  
4. Vision-Based Autonomous Surface Vehicles  
5. Deep Learning for Marine Environment Perception  

---

## Proje Yapısı


