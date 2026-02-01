# Fetal Health Classification Project

## Proje Hakkında
Bu projede, fetal sağlık durumunun sınıflandırılması amacıyla farklı makine öğrenmesi algoritmaları kullanılmıştır. Amaç; verilen klinik ölçümlerden yola çıkarak fetüsün sağlık durumunu **Normal**, **Suspect** veya **Pathological** olarak tahmin edebilen bir model geliştirmektir.

Projede sınıflandırma problemleri için yaygın olarak kullanılan yöntemler uygulanmış ve sonuçları karşılaştırılmıştır.

---

## Kullanılan Veri Seti
Projede **Fetal Health Dataset** kullanılmıştır.  
Veri seti; kalp atım hızı, kasılmalar, varyasyon ölçümleri ve histogram tabanlı özellikler gibi toplam 21 öznitelikten oluşmaktadır.

Hedef değişken:
- `fetal_health`
  - 1: Normal
  - 2: Suspect
  - 3: Pathological

Eksik veri kontrolü yapılmış ve veri setinde eksik gözlem olmadığı görülmüştür.

---

## Kullanılan Yöntemler
Projede aşağıdaki sınıflandırma algoritmaları kullanılmıştır:
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- Decision Tree

Modeller Accuracy, Precision, Recall ve F1-Score metrikleri kullanılarak değerlendirilmiştir.

---

## Projenin Çalıştırılması
1. Anaconda kurulumu yapılır.
2. Gerekli kütüphaneler yüklenir:
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn
4.analysis.ipynb dosyası Jupyter Notebook üzerinden açılır.
5. Hücreler sırasıyla çalıştırılarak:
Veri analizi
Model eğitimi
Performans değerlendirmeleri yapılır.

## Sonuçlar

Uygulanan modeller karşılaştırıldığında en yüksek başarıyı Decision Tree modeli göstermiştir.
Bu model, özellikle patolojik vakaların doğru sınıflandırılmasında diğer modellere göre daha iyi sonuçlar vermiştir.

Sağlık verilerinde kritik öneme sahip olan Recall ve F1 Score değerleri dikkate alındığında Decision Tree modeli en güvenilir model olarak seçilmiştir.

## Kullanılan Teknolojiler
Python
Pandas, NumPy
Scikit-learn
Matplotlib, Seaborn