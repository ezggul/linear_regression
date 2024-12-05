# linear_regression
Bu projede ünlü bir kozmetik markasının 2014 yılı boyunca Facebook sayfasında yayınlanan gönderilerine ilişkin oluşturulmuş bir veri setini kullanarak doğrusal regresyon modeli oluşturacağız. Bu veri setindeki seçilen bazı özellikleri (sütunları) kullanarak bir model eğiteceğiz. Bu özellikleri seçerken dikkatli olunması gerekir. Çünkü aşırı öğrenme ya da öğrenmeme problemleriyle karşılaşabiliriz. Bu gibi durumlarda modelimizin tahmini gerçek değerinden çok farklı çıkacaktır, istenmeyen bir durumdur. 
Doğrusal, bir diğer adıyla Lineer Regresyon, ilgili ve bilinen başka bir veri değeri kullanarak bilinmeyen verilerin değerini tahmin eden bir veri analizi tekniğidir.


Araştırma Problemi: 

Python programlama dilini kullanarak verilen veri setiyle Doğrusal Regresyon kodu yazılacaktır.

Veri Seti: Facebook Posts Metrics 

Veri Seti Öznitelikleri: 
• Kategori, 
• Sayfa toplam beğenisi: Şirketin sayfasını beğenen kişi sayısı), 
• Tür: İçerik türü (Bağlantı, Fotoğraf, Durum, Video), 
• Gönderi ayı: Gönderinin yayınlandığı ay (Ocak, Şubat, Mart,…, Aralık), 
• Gönderim saati: Gönderinin yayınlandığı saat (0, 1, 2, 3, 4, …, 23), 
• Hafta içi gönderi: Gönderinin yayınlandığı hafta içi (Pazar, Pazartesi, …, Cumartesi), 
• Ücretli: Şirketin reklam için Facebook'a ödeme yapması durumunda (evet, hayır) 

Modelimizde ilk kullanacağımız özellikler: 
Modellemeye çalışabileceğimiz birçok olası özellik var ancak biz “Total Interactions” ‘e odaklanacağız. Özellik alanımız şunları içerecektir: “Category”, “Page total likes”, “Post month”, “Post hour”, “Post weekday”, “Type” ve “Paid”. 
Takip Ettiğimiz Adımlar: 

• Verinin indirilmesi 

• Verinin okunması: Veri seti modelimize aktarılarak, istediğimiz özelliklere göre şekillendirildi. Null değerleri dolduruldu.

• Verileri Bölme (X ve Y (X_train, X_Test ve y_train, y_test)) 
a. Veri kümesini X ve Y'ye bölündü. 
b. Sağlanan yüzdesel bölmeyi kullanarak X ve Y'yi eğitim ve test setlerine ayrıldı (varsayılan, %80 eğitim ve %20 testtir). 

• Doğrusal regresyon fonksiyonunu oluşturabilmek için gerekli araştırmalar yapıldı. Matematiksel olarak anlaşılarak gerekli sınıf içinde fonksiyonlar oluşturuldu.

• Modelin eğitimi ve test edilmesi 
a. train_test_split() öğesini çağrılarak eğitim ve test seti alındı.
b. Bir ağırlık (θ) vektörü tanımlandı.
c. Yukarıdaki bilgiler kullanılarak Gradyan İnişini (Gradient Descent) uygulandı.
d. Eğitim ve test verileri için Toplam Kare Hata (Sum Squared Error) kaydedildi. 
e. Ağırlık matrisi, eğitim hataları ve test hataları döndürüldü.
f. Eğitim ve test hataları çizildi. Grafikte aşırı öğrenme gerçekleştiği için farklı sütunlarla yeniden denendi.
