## 🚗 Arabam.com Web Scraping & Fiyat Tahmin Modeli
Bu projede, arabam.com sitesinden araçlara ait veriler web scraping yöntemiyle çekilmiş, ardından bu verilerle fiyat tahmini yapılmıştır. Modellemelerde hem RandomForestRegressor hem de OLS (Ordinary Least Squares) regresyonu kullanılmıştır.

## 📦 Dosya Yapısı

| Dosya Adı         | Açıklama |
|------------------|----------|
| `WSarabamCom.ipynb` | Web scraping işlemini gerçekleştiren Jupyter notebook |
| `arabalar.xlsx`     | Arabam.com’dan çekilen ham veri |
| `Untitled.ipynb`    | Veri ön işleme, görselleştirme ve modelleme yapılan dosya |
---

### 🔧 Kullanılan Teknolojiler:
* 🕷️ Web Scraping: requests, BeautifulSoup

* 📊 Veri İşleme: pandas, numpy

* 📈 Modelleme: scikit-learn, statsmodels

* 🎨 Görselleştirme: matplotlib, seaborn

### 🔎 Özellikler:
* ✔️ Veri ön işleme: Eksik veri temizleme, encoding, normalizasyon

* ✔️ Model karşılaştırması: OLS vs RandomForest

* ✔️ Performans metrikleri: R², RMSE

* ✔️ Tahmin sonuçları & görseller

* ✔️ Kullanıcıya öneri yapılabilecek tahmin sistemi altyapısı

### 📊 Model Skorları:
##### 🎯 Random Forest
* R² Skoru: 0.9199

* RMSE: 376452.54

##### 📉 OLS Regresyon
* R² Skoru: 0.589

💡 Yorum:
RandomForestRegressor, klasik OLS modeline kıyasla çok daha yüksek bir başarı oranı sağlamış.

OLS modeli, değişkenlerin anlamlılığını istatistiksel olarak test etmek için faydalı olurken, tahmin başarısı açısından Random Forest modeli açık ara önde.

RMSE değeri, modelin fiyat tahmininde yaklaşık ±376K TL hata payı olduğunu göstermektedir (daha da iyileştirilebilir).
