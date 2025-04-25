ARABAM.COM İLAN ANALİZİ - README

 PROJE ÖZETİ
Bu proje, Türkiye'nin en popüler ikinci el araç alım-satım platformlarından biri olan Arabam.com'dan web scraping yöntemiyle toplanan ilan verilerinin analizini kapsamaktadır. Amaç, araç fiyatlarını etkileyen temel faktörleri tespit etmek ve bu faktörlere dayanarak güçlü bir fiyat tahmin modeli geliştirmektir. 

Proje aynı zamanda, analiz sonuçlarının kullanıcıya daha anlaşılır sunulabilmesi için Dash (Python tabanlı web framework) ile görselleştirme uygulaması ve Power BI ile interaktif bir dashboard tasarımını da içermektedir. Böylece hem veri bilimi temelli bir analiz yapılmış hem de karar destek sistemlerine katkı sağlayacak bir çözüm ortaya konmuştur.

 PROJENİN AMACI
- Araç fiyatlarını etkileyen değişkenleri (kilometre, yıl, motor gücü, kasa tipi, marka, model, renk, çekiş türü vb.) analiz etmek,
- Bu değişkenler üzerinden bir regresyon modeli kurarak fiyat tahmini yapmak,
- Modelin başarımını değerlendirerek farklı hata metrikleriyle sonuçları yorumlamak,
- Elde edilen içgörüleri, Dash ve Power BI gibi araçlarla kullanıcıya etkileşimli ve görsel olarak sunmak.

 VERİ SETİ HAKKINDA
- Kaynak: www.arabam.com
- Tarih: Mart 2025
- Toplam Filtrelenmiş Girdi: 580 ilan
- Veri Toplama Yöntemi: Web scraping (requests, BeautifulSoup)
- Eksik Veriler: Ortalama ve Random Forest ile doldurulmuştur.
- Not: İlanlar zamanla yayından kalkmış veya içerik olarak değişmiş olabilir. Bu analiz yalnızca Mart 2025'teki durumu yansıtır.

 DEĞİŞKENLER (Özellikler)
- Marka
- Model
- Üretim Yılı
- Kilometre
- Motor Gücü (hp)
- Kasa Tipi (sedan, hatchback vs.)
- Çekiş Türü (ön, arka, 4x4)
- Renk
- Fiyat (TL)

 YAPILAN ANALİZLER
- Araç fiyatlarının dağılımı
- Kilometre – fiyat ilişkisi
- Yıl – fiyat ilişkisi
- Motor gücü – fiyat ilişkisi
- Kasa tipi & çekiş kombinasyonlarının fiyat üzerindeki etkisi
- Renk tercihlerinin fiyatlara etkisi
- Korelasyon analizi
- Feature engineering
- Outlier (aykırı değer) temizleme
- Random Forest regresyon modeli ile fiyat tahmini
- Alternatif model denemeleri (Linear Regression, Decision Tree, XGBoost)
- Model performans değerlendirmesi

 MODEL PERFORMANSI (Random Forest Regressor)
- R² (Determinasyon Katsayısı): 0.7032
- MSE (Mean Squared Error): 105,452,970,738.19
- RMSE (Root MSE): 324,735.23
- MAE (Mean Absolute Error): 172,583.65
- MAPE (Mean Absolute Percentage Error): %10.55

 DASHBOARD VE GÖRSELLEŞTİRME
 Python Dash:
- Filtrelenebilir grafikler (marka, kasa tipi, motor gücü, yıl vb.)
- Anlık değişen fiyat dağılımları
- Dinamik fiyat tahminleri

 Power BI:
- Interaktif bar, scatter, box ve line chart’lar
- İl bazlı araç dağılım haritası
- Kategori bazlı özet tablolar
- Öne çıkan marka-model analizleri



 KATKIDA BULUNANLAR
- Onur Atik – Veri Toplama, Web Scraping, Veri Analizi, Modelleme, Dash Geliştirme, Raporlama

 NOTLAR
- Bu proje, istatistik, makine öğrenmesi ve görselleştirme tekniklerini bir arada kullanarak gerçek dünya verisiyle çözüm üretme örneğidir.
- Kodlar açık kaynaklıdır ve geliştirilmeye açıktır.
- Daha iyi sonuçlar için farklı modeller, hiperparametre ayarlamaları ve daha geniş veri setleri denenebilir.
