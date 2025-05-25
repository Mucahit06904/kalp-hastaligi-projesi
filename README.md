Akbank Makine Öğrenmesi Bootcamp – Kalp Hastalığı Tahmin Projesi
1. Proje Tanımı
Bu projede, kalp hastalığı tahminini amaçlayan bir makine öğrenmesi modeli geliştirilmiştir. Veri seti üzerinde gözetimli öğrenme teknikleri kullanılarak, hastaların kalp hastalığı durumu (var/yok) sınıflandırılmıştır.
Amaç, hastaların özelliklerine göre kalp hastalığı riskini tahmin ederek erken teşhis ve sağlık yönetimine katkı sağlamaktır.
________________________________________
2. Veri Seti
Kullanılan veri seti: Heart Failure Prediction Dataset
Kaynak: Kaggle
Veri seti 918 hasta verisi içermekte olup, aşağıdaki özellikleri kapsamaktadır:
•	Age (Yaş)
•	Sex (Cinsiyet)
•	ChestPainType (Göğüs Ağrısı Tipi)
•	RestingBP (Dinlenme Tansiyonu)
•	Cholesterol (Kolesterol)
•	FastingBS (Açlık Kan Şekeri)
•	RestingECG (Dinlenme ECG Sonucu)
•	MaxHR (Maksimum Kalp Hızı)
•	ExerciseAngina (Egzersiz Anjinası)
•	Oldpeak (Egzersizle İlgili ST Depresyonu)
•	ST_Slope (ST Eğim)
•	HeartDisease (Hedef Değişken, Kalp Hastalığı Durumu)
________________________________________
3. Keşifsel Veri Analizi (EDA)
•	Veri setinde eksik değer bulunmamaktadır.
•	Korelasyon matrisi ile değişkenler arasındaki ilişkiler incelendi. Özellikle yaş, maksimum kalp hızı ve egzersizle ilgili değişkenlerin hedef değişkenle ilişkisi yüksek bulundu.
•	Kalp hastalığı dağılımında sınıf dengesizliği hafif seviyededir.
•	Kategorik değişkenlerin kalp hastalığı ile ilişkileri grafiklerle gösterildi.
________________________________________
4. Veri Ön İşleme
•	Kategorik değişkenler one-hot encoding ile sayısal verilere dönüştürüldü.
•	Veriler eğitim ve test setlerine %80 - %20 oranında ayrıldı.
•	Özellikler StandardScaler ile ölçeklendirildi.
________________________________________
5. Model Geliştirme
•	Başlangıçta Lojistik Regresyon modeli kullanıldı.
•	Model doğruluğu test setinde yaklaşık %84 olarak elde edildi.
•	Hiperparametre optimizasyonu için GridSearchCV kullanıldı.
•	En iyi parametrelerle model doğruluğu %85 seviyesine yükseldi.
•	Ayrıca Random Forest modeli ile özellik önemleri analiz edildi.
________________________________________
6. Model Değerlendirme
•	Doğruluk (Accuracy), Kesinlik (Precision), Duyarlılık (Recall), F1 Skoru gibi metrikler hesaplandı.
•	Karışıklık matrisi ve ROC eğrisi ile model performansı görselleştirildi.
•	Eğitim ve test doğrulukları karşılaştırılarak modelin aşırı öğrenme yapmadığı kontrol edildi.
________________________________________
7. Sonuç ve Öneriler
•	Geliştirilen model, kalp hastalığı tahmininde etkili sonuçlar vermiştir.
•	Bu model, sağlık kurumlarında erken teşhis için destekleyici bir araç olarak kullanılabilir.
•	Gelecekte modele daha fazla veri eklenerek ve derin öğrenme teknikleri kullanılarak iyileştirmeler yapılabilir.
•	Ayrıca aynı veri seti üzerinde gözetimsiz öğrenme (örneğin K-means kümeleme) yöntemleriyle hasta gruplaması çalışmaları yapılabilir.
•	Projenin web arayüzü veya mobil uygulama haline getirilerek pratik kullanımı artırılabilir.
________________________________________
8. Proje Kaynakları ve Linkler
•	Kaggle Notebook: [Kaggle Notebook Editor](https://www.kaggle.com/code/mcahitsarca/notebookdb23e98211/edit)
•	Veri Seti: https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction
•	GitHub Repo: https://github.com/yourusername/heart-disease-prediction
________________________________________
Ek Bilgiler
•	Projede Python, Pandas, Scikit-learn, TensorFlow, Matplotlib ve Seaborn kütüphaneleri kullanılmıştır.
•	Model eğitimi ve değerlendirmesi Kaggle ortamında gerçekleştirilmiştir.
________________________________________
Teşekkürler
Akbank Makine Öğrenmesi Bootcamp ve Kaggle topluluğuna teşekkür ederim.

