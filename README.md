# 🚢 Titanic Survival Prediction (Machine Learning)

Bu proje, tarihi Titanic veri setini kullanarak yolcuların hayatta kalma olasılıklarını tahmin eden bir makine öğrenmesi modelidir.

## 🎯 Proje Hakkında
Makine öğrenmesinde **Sınıflandırma (Classification)** problemi olarak ele alınan bu çalışmada; yolcuların yaşı, cinsiyeti, bilet sınıfı gibi öznitelikler kullanılarak hayatta kalıp kalamayacakları analiz edilmiştir.

## 🛠 Kullanılan Teknolojiler
* **Python**
* **Pandas & NumPy:** Veri manipülasyonu ve temizliği.
* **Seaborn & Matplotlib:** Veri görselleştirme.
* **Scikit-Learn:** Makine öğrenmesi modeli (Decision Tree Classifier).

## 📊 Proje Adımları
1. **Veri Temizliği (Data Cleaning):**
   - Eksik yaş verileri (Missing Values), veri setinin genel ortalaması ile dolduruldu (**Mean Imputation**).
   - Analize katkısı olmayan sütunlar (`deck`, `adult_male` vb.) temizlendi.
2. **Öznitelik Mühendisliği (Feature Engineering):**
   - Kategorik veriler (Kadın/Erkek, Limanlar) **One-Hot Encoding** yöntemiyle sayısal verilere (0/1) çevrildi.
3. **Modelleme:**
   - Veri seti **%80 Eğitim**, **%20 Test** olarak ayrıldı.
   - **Decision Tree (Karar Ağacı)** algoritması kullanılarak model eğitildi.

## 🏆 Sonuçlar
Model, test verisi üzerinde **%76.40 Doğruluk (Accuracy)** oranına ulaşmıştır.
* **Keşif:** Modelin karar ağacı incelendiğinde, hayatta kalmayı etkileyen en önemli faktörün **"Cinsiyet"** (Kadın olmak) olduğu, bunu **"Bilet Sınıfı"**nın takip ettiği görülmüştür.

---
