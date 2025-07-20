📊 Sigorta Verisi Üzerinde Makine Öğrenmesi Projesi
Bu projede, Kaggle üzerinden alınan bir sigorta verisi seti kullanılarak veri ön işleme, görselleştirme ve makine öğrenmesi modelleme süreçleri uygulanmıştır. Amaç, bireylerin sigorta masraflarını tahmin etmektir.

🔍 Kullanılan Veri Seti
insurance.csv adlı veri seti kullanılmıştır.

Değişkenler:

age: Yaş

sex: Cinsiyet

bmi: Vücut kitle indeksi

children: Çocuk sayısı

smoker: Sigara içme durumu

region: Bölge

charges: Sigorta masrafı (bağımlı değişken)

🧹 1. Veri Ön İşleme
Eksik Veri Kontrolü: Veri setinde eksik veri bulunmadığı tespit edilmiştir.

Kategorik Değişkenler: sex, smoker ve region değişkenleri One-Hot Encoding ile sayısallaştırılmıştır.

Outlier Analizi: bmi ve charges değişkenleri için boxplot grafikleri çizilerek aykırı değerler incelenmiştir.

Aykırı Değer Temizliği: Belirlenen eşiklere göre bazı aykırı değerler veri setinden kaldırılmıştır.

📊 2. Görselleştirmeler
Dağılım Grafikleri: age, bmi, charges gibi değişkenlerin dağılımı incelenmiştir.

Korelasyon Matrisi: Sayısal değişkenler arasındaki korelasyonlar görselleştirilmiştir.

Sigara ve Masraf İlişkisi: Sigara içenlerin sigorta ücretinin daha yüksek olduğu gösterilmiştir.

Bölge Bazlı Masraf Analizi: Sigorta ücretlerinin bölgelere göre farklılık gösterip göstermediği incelenmiştir.

🤖 3. Modelleme
Bağımlı Değişken: charges

Modeller:

Linear Regression

Ridge Regression

Lasso Regression

Decision Tree Regressor

Random Forest Regressor

Veri Ayrımı:

Train/Test Split (%80/%20)

Değerlendirme Metrikleri:

RMSE (Root Mean Squared Error)

RMSLE (Root Mean Squared Logarithmic Error)

📈 4. Model Performansı
Her model için eğitim ve test hataları ayrı ayrı hesaplanmıştır.

Overfitting kontrolü yapılmıştır.

En iyi performans gösteren model Random Forest olarak seçilmiştir.

📌 Ekstra Adımlar
Ridge ve Lasso modelleri için alpha parametresiyle denemeler yapılmıştır.

Box-Cox dönüşümü ile normalleştirme uygulanarak model performansı artırılmaya çalışılmıştır.

