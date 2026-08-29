# 🤖 Machine Learning Model Evaluation & Classification Performance

Bu depoda, farklı makine öğrenmesi algoritmalarının (`Support Vector Classifier`, `Logistic Regression` ve `Gaussian Naive Bayes`) sınıflandırma performansları detaylı bir şekilde test edilmiş; confusion matrix, classification report ve ROC-AUC eğrileri üzerinden karşılaştırmalı analizleri yapılmıştır.

## 🛠️ Kullanılan Teknolojiler

* **Python 3**
* **Scikit-Learn** (Modelleme ve Metrik Hesaplama)
* **Matplotlib & Seaborn** (Görselleştirme)

---

## 📊 Model Performansları ve Karşılaştırmalı Analiz

### 1. Support Vector Classifier (SVC - RBF Kernel)
SVC modeli, dengesiz veri setlerinde ve karmaşık karar sınırlarında yüksek performans göstermiştir. Özel eşik değeri (`threshold = 0.25`) ile yapılan değerlendirmede model, dengeli bir precision ve recall dengesi yakalamıştır.

* **Confusion Matrix ve Classification Report:**
<p align="center">
  <img src="images/SVCRESULTS_6.png" width="700" alt="SVC Results">
</p>

* **ROC Eğrisi ve AUC Skoru:** Model **0.9217** gibi oldukça yüksek bir AUC skoru elde ederek sınıflandırma yeteneğinin ne kadar güçlü olduğunu kanıtlamıştır.
<p align="center">
  <img src="images/SVCROCCURVE_5.png" width="700" alt="SVC ROC Curve">
</p>

---

### 2. Logistic Regression
Doğrusal sınıflandırma problemlerinin vazgeçilmezi olan Lojistik Regresyon modeli, özel eşik optimizasyonuyla birlikte test edilmiştir.

* **Confusion Matrix ve Classification Report:**
<p align="center">
  <img src="images/LogRegResults_6.png" width="700" alt="Logistic Regression Results">
</p>

* **ROC Eğrisi ve AUC Skoru:** Model **0.8265** AUC skoru ile genel eğri altında başarılı bir performans sergilemiştir.
<p align="center">
  <img src="images/LogRegROCCurve_6.png" width="700" alt="Logistic Regression ROC Curve">
</p>

---

### 3. Gaussian Naive Bayes (GaussianNB)
Olasılıksal temelli yaklaşımıyla bilinen GaussianNB modeli, hızlı sonuçlar üretebilmesine rağmen azınlık sınıfındaki (`1` sınıfı) yakalama oranında (recall) diğer modellere nazaran daha düşük kalmıştır.

* **Confusion Matrix ve Classification Report:**
<p align="center">
  <img src="images/GaussianNBRESULTS_6.png" width="700" alt="GaussianNB Results">
</p>

* **ROC Eğrisi ve AUC Skoru:** Model **0.8638** AUC skoruna ulaşmıştır.
<p align="center">
  <img src="images/GaussianNBROCCURVE_6.png" width="700" alt="GaussianNB ROC Curve">
</p>

---

## 🚀 Projeyi Çalıştırma

Kodları kendi bilgisayarınızda çalıştırmak ve sonuçları tekrarlamak için:

1. Depoyu klonlayın:
   ```bash
   git clone [https://github.com/SemihBatin/Machine-Learning-Model-Evaluation-Classification-Performance.git](https://github.com/SemihBatin/Machine-Learning-Model-Evaluation-Classification-Performance.git)
