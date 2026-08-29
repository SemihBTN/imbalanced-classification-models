# imbalanced-classification-models

# 🤖 Machine Learning Model Evaluation & Classification Performance

Bu depoda, farklı makine öğrenmesi algoritmalarının (`Support Vector Classifier`, `Logistic Regression` ve `Gaussian Naive Bayes`) sınıflandırma performansları detaylı bir şekilde test edilmiş; confusion matrix, classification report ve ROC-AUC eğrileri üzerinden karşılaştırmalı analizleri yapılmıştır.

## 🛠️ Kullanılan Teknolojiler

* **Python 3**
* **Scikit-Learn** (Modelleme ve Metrik Hesaplama)
* **Matplotlib & Seaborn** (Görselleştirme)

---

## 📊 Model Performansları ve Karşılaştırmalı Analiz

### 1. Support Vector Classifier (SVC - RBF Kernel)
SVC modeli, dengesiz veri setlerinde ve karmaşık karar sınırlarında yüksek performans göstermiştir. Özel eşik değeri (`threshold = 0.25`) ile yapılan değerlendirmede model, dengeli bir precision ve recall dengesi yakalamıştır[cite: 9].

* **Confusion Matrix ve Classification Report:**
<p align="center">
  <img src="images/SVCRESULTS_2.png" alt="SVC Results" width="75%"/>
</p>

* **ROC Eğrisi ve AUC Skoru:** Model **0.9217** gibi oldukça yüksek bir AUC skoru elde ederek sınıflandırma yeteneğinin ne kadar güçlü olduğunu kanıtlamıştır.
<p align="center">
  <img src="images/SVCROCCURVE.png" alt="SVC ROC Curve" width="75%"/>
</p>

---

### 2. Logistic Regression
Doğrusal sınıflandırma problemlerinin vazgeçilmezi olan Lojistik Regresyon modeli, özel eşik optimizasyonuyla birlikte test edilmiştir.

* **Confusion Matrix ve Classification Report:**
<p align="center">
  <img src="images/LogRegResults_2.png" alt="Logistic Regression Results" width="75%"/>
</p>

* **ROC Eğrisi ve AUC Skoru:** Model **0.8265** AUC skoru ile genel eğri altında başarılı bir performans sergilemiştir.
<p align="center">
  <img src="images/LogRegROCCurve_2.png" alt="Logistic Regression ROC Curve" width="75%"/>
</p>

---

### 3. Gaussian Naive Bayes (GaussianNB)
Olasılıksal temelli yaklaşımıyla bilinen GaussianNB modeli, hızlı sonuçlar üretebilmesine rağmen azınlık sınıfındaki (`1` sınıfı) yakalama oranında (recall) diğer modellere nazaran daha düşük kalmıştır.

* **Confusion Matrix ve Classification Report:**
<p align="center">
  <img src="images/GaussianNBRESULTS_2.png" alt="GaussianNB Results" width="75%"/>
</p>

* **ROC Eğrisi ve AUC Skoru:** Model **0.8638** AUC skoruna ulaşmıştır.
<p align="center">
  <img src="images/GaussianNBROCCURVE_2.png" alt="GaussianNB ROC Curve" width="75%"/>
</p>

---

## 🚀 Projeyi Çalıştırma

Kodları kendi bilgisayarınızda çalıştırmak ve sonuçları tekrarlamak için:

1. Depoyu klonlayın:
    ```bash
    git clone [https://github.com/SemihBatın/Machine-Learning-Model-Evaluation-Classification-Performance.git](https://github.com/SemihBatın/Machine-Learning-Model-Evaluation-Classification-Performance.git)
    ```
2. Gerekli kütüphaneleri yükleyin:
    ```bash
    pip install pandas numpy scikit-learn matplotlib seaborn
    ```
3. Jupyter Notebook ortamını başlatarak adımları sırasıyla çalıştırabilirsiniz.
