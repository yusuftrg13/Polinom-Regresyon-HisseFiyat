# Polinom-Regresyon-HisseFiyat
Polinom Regresyon ile THYAO Hisse Fiyat Tahmini
Bu proje, THYAO hisse senedi fiyatlarını Polinom Regresyon kullanarak tahmin etmeyi amaçlamaktadır. Projede, Python ve popüler veri bilimi kütüphanelerini (Pandas, NumPy, scikit-learn, Matplotlib) kullanarak hisse fiyatlarının doğrusal olmayan değişimlerini modelledik.

Proje Yapısı
Veri Yükleme ve İşleme:

THY.csv dosyasından THYAO hisse fiyat verilerini çektik.
Fiyat verilerini sayısal formata çevirdik (örneğin, virgülleri noktaya çevirerek).
Tarihleri günlük sıraya göre numaralandırdık, böylece fiyat tahmini için polinom özellikler ekleyebildik.
Özellik Mühendisliği - Polinom Özellikleri:

Zamanın etkisini modele dahil etmek için günlük sıraya göre 3. dereceden polinom özellikler oluşturduk.
Polinom özellikler, doğrusal olmayan eğilimleri daha iyi modellememizi sağladı.
Model Eğitimi:

scikit-learn’ün LinearRegression sınıfını kullanarak model eğitimi gerçekleştirdik.
Modelimizi eğitim ve test setlerine ayırarak eğitim gerçekleştirdik.
Model Performansını Değerlendirme:

Modeli Mean Squared Error (MSE) ve R-squared (R²) metrikleri ile değerlendirdik.
Modelin doğruluğunu, gerçek fiyatlarla tahmin edilen fiyatları karşılaştırarak analiz ettik.
Sonuçların Görselleştirilmesi:

Gerçek fiyatlarla modelin tahmin ettiği fiyatları bir grafik üzerinde görselleştirdik.
Kullanılan Başlıca Kütüphaneler
pandas: Veri yükleme ve işleme
numpy: Nümerik işlemler
scikit-learn: Model eğitimi ve değerlendirme
matplotlib: Grafik ve görselleştirme
