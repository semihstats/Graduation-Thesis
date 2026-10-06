# AAPL Getiri Tahmini

Bu depo, Apple (AAPL) hissesinin bir sonraki işlem günündeki log getirisini
tahmin etmeye yönelik mezuniyet tezinin kodlarını ve deney çıktılarını içerir.
Çalışmada klasik makine öğrenmesi modelleri, derin öğrenme modelleri ve hibrit
CNN-BiLSTM modeli karşılaştırılmaktadır.

## Proje içeriği

- `veri_kesfi_temizleme.ipynb` - finansal verilerin keşfi, kalite kontrolleri,
  temizlenmesi ve veri setinin hazırlanması.
- `makine_ogrenimi_modelleri.ipynb` - Linear Regression, Decision Tree,
  Random Forest, Gradient Boosting, k-NN, SVR, XGBoost ve LightGBM modelleri.
- `derin_ogrenme_modelleri.ipynb` - CNN, LSTM ve BiLSTM deneyleri.
- `cnn_bilstm_hibrit.ipynb` - çok ölçekli hibrit CNN-BiLSTM modeli.
- `data/` - ham ve temizlenmiş AAPL veri setleri.
- `saved_models/` - eğitilmiş Keras model dosyaları.

Modeller değerlendirilirken gelecek gözlemlerin kullanılmasını önlemek için
kronolojik eğitim ve test ayrımı uygulanmıştır. Performans; MSE, RMSE ve MAE
gibi regresyon metrikleriyle raporlanmaktadır.

## Kurulum ve çalıştırma

1. Bir Python ortamı oluşturun ve gerekli paketleri yükleyin:

   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn tensorflow xgboost lightgbm yfinance jupyter
   ```

2. Depo kök dizininde Jupyter Notebook'u başlatın:

   ```bash
   jupyter notebook
   ```

3. Notebook'ları aşağıdaki sırayla çalıştırın:

   1. `veri_kesfi_temizleme.ipynb`
   2. `makine_ogrenimi_modelleri.ipynb`
   3. `derin_ogrenme_modelleri.ipynb`
   4. `cnn_bilstm_hibrit.ipynb`

Temizlenmiş veri seti ve önceden eğitilmiş modeller depoya dahil edilmiştir.
Bu nedenle model notebook'ları depo kök dizininden açıldığında doğrudan
çalıştırılabilir.


