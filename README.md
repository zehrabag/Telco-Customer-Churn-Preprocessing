# Telco Customer Churn Veri Ön İşleme ve Analizi

Bu depo, bir telekomünikasyon şirketinin müşteri terk oranını (Churn) tahmin etmeyi amaçlayan bir makine öğrenimi projesinin **veri ön işleme (Data Preprocessing)** aşamalarını kapsamaktadır. Proje, popüler bir Kaggle veri seti olan Telco Customer Churn verilerini kullanmaktadır.

Veri setini makine öğrenimi modellerine hazır hale getirmek için zorunlu olan temizleme, dönüşüm ve ölçeklendirme adımlarının tamamı Python ve ilgili kütüphaneler (Pandas, Scikit-learn, Imbalance-learn) ile uygulanmıştır.

## 🚀 Uygulanan Ana Adımlar ve Teknikler

| Aşama | Uygulanan Teknikler | Amaç |
| :--- | :--- | :--- |
| **Veri Temizleme** | Eksik Değer Doldurma (Medyan), Hatalı Veri Tipi Düzeltme, Gereksiz Sütun Kaldırma (`customerID`). | Tutarsız ve eksik verileri modellemeye uygun hale getirmek. |
| **Veri Dönüştürme** | One-Hot Encoding (Çoklu Kategorik), Binary Encoding (İkili Kategorik), Logaritmik Dönüşüm (`TotalCharges`). | Kategorik verileri sayısal formatlara çevirmek ve çarpık dağılımları normale yaklaştırmak. |
| **Özellik Ölçeklendirme** | **Min-Max Normalizasyon**, **Z-Score Standardizasyonu**, **Robust Scaling**. | Farklı ölçeklerdeki sayısal özellikleri standart bir aralığa getirmek. |
| **Veri Örnekleme** | **SMOTE (Synthetic Minority Oversampling Technique)**. | Dengesiz (Imbalanced) olan hedef değişkenin (`Churn`) sınıflarını dengelemek. |

## 📦 Kullanılan Kütüphaneler

* `pandas`
* `numpy`
* `matplotlib`
* `seaborn`
* `scikit-learn` (Ölçekleyiciler için)
* `imbalanced-learn` (SMOTE için)

## ✨ Görselleştirme Sonuçları

Uygulanan her ön işleme adımının etkisi, dağılım grafikleri (Log Dönüşümü) ve sayım grafikleri (SMOTE) kullanılarak görsel olarak analiz edilmiş ve sonuçları doğrulanmıştır.
