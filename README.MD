
BT Akaaemi/ Career HuBT – Veri Bilimi Eğitimi Ders Notlarım

# PyPI ile Veri Setleri Kullanımı

1.PyPI'den Veri Setlerini Bulmak ve Kurmak

[PyPI](https://pypi.org/) (Python Package Index) sitesine gidin.

Arama çubuğuna `"data sets"` yazın ve `datasets 3.0.1` paketini bulun.
Bu paketi kurmak için terminal veya komut satırında şu komutu kullanın:

*pip install datasets

2.Değişken Tanımlama ve Atama:

Örnek

İsim adlı bir değişkene "Selcen" değerini atayın:

İsim = "Selcen"

3.Değişkeni Güncelleme

Bu değişkene "Ali" değerini atayarak değiştirebilirsiniz:

İsim = "Ali"


# Koleksiyonlar (collections)/Veri Koleksiyonları
## Listeler (List) / Array / Dizi / Series / Katar

- `meyveler` listesi:

  ```python
  meyveler = ["elma", "armut", "muz", "kivi", "çilek", "çilek"]

*Sınıf isim listeleri:

sinif_isim_listeleri = [["ali", "ayşe"], ["mehmet", "gizem"]]

*Liste uzunluğunu hesaplama:
len(meyveler)

*Kümeler (Set)

meyve_kumesi = {"elma", "armut", "muz", "kivi", "çilek", "çilek"}

*Sözlük Yapısı (Dictionary, Map, Hashmap)
meyve_sozluk = {"elma": "ingilizcesi apple olan kışlık bir meyve", "armut": "ingilizcesi pear olan yazlık bir meyve"}

###Kümeler (Set) ve Özellikleri

Tanım: Küme (set) veri yapısı, bir koleksiyonun benzersiz (yani tekrarsız) elemanlardan oluşmasını sağlar. Kümelerdeki elemanların sırası önemli değildir ve her eleman sadece bir kez yer alır.

Tekrarsız Elemanlar: {"elma", "armut", "muz", "kivi", "çilek", "çilek"} kümesinde iki adet "çilek" olduğu halde, kümede yalnızca bir kez "çilek" bulunur. Bu nedenle, kümeye eklediğimiz iki "çilek" değeri yalnızca bir tane "çilek" olarak saklanır.

Çıkış İşlemi: Küme elemanlarını ekledikten sonra, print(meyve_kumesi) komutunu çalıştırdığımızda, {‘armut’, ‘elma’, ‘kivi’, ‘muz’, ‘çilek’} çıktısını görürüz. Bu çıktıda elemanlar sırasız şekilde ve tekrarsız olarak listelenmiştir.


#Proje Adı: Reno Clio Yaş ve Kilometre Analizi

1.Amaç:
Bu projede, Reno Clio araçlarının yaşları ve kilometre bilgileri arasındaki ilişkiyi incelemek ve lineer regresyon modeli kullanarak bir tahminleme sistemi oluşturmak amaçlanmıştır.

2.Veri Seti:
reno_clio.csv: Bu dosya, araçların yaş ve kilometre bilgilerini içeren verileri tutar.

3.Veri Hazırlığı:
**Veri Yükleme: pandas kütüphanesi kullanılarak "reno_clio.csv" dosyası okunmuş ve bir DataFrame'e yüklenmiştir.
**Yaş Hesaplama: Araçların yaşları, mevcut yıldan üretim yıllarının çıkarılmasıyla hesaplanmıştır.

5.Veri Analizi:

**Veri Görselleştirme:
Araçların yaş ve kilometre bilgileri, bir scatter plot ile görselleştirilmiştir. Bu grafik, iki değişken arasındaki genel ilişkiyi göstermektedir.

**Lineer Regresyon:
sklearn.linear_model kütüphanesinden LinearRegression modeli kullanarak, araç yaşı ve kilometresi arasında doğrusal bir ilişki kurulmuştur.
Modelin katsayıları (a ve b) hesaplanmıştır. Bu katsayılar, y = ax + b doğrusal denklemindeki parametreleri temsil eder.
Elde edilen model kullanılarak, belirli bir yaştaki bir araç için tahmini kilometre değeri hesaplanmıştır.

**Model Değerlendirmesi:
Eğitim verileri üzerinde yapılan tahminler, gerçek değerlerle karşılaştırılarak modelin performansı değerlendirilmiştir.

6.Sonuçlar:
Araç yaşı ile kilometre arasında pozitif bir korelasyon olduğu gözlemlenmiştir. Yani, araç yaşı arttıkça kilometresi de artma eğilimindedir.

Oluşturulan lineer regresyon modeli, verileri genel olarak iyi bir şekilde açıklamaktadır. Ancak, modelin doğruluğu, daha fazla veri ve farklı modellerle incelenerek iyileştirilebilir.

***Kullanılan Kütüphaneler:

pandas: Veri analiz ve manipülasyonu için.
matplotlib: Veri görselleştirme için.
sklearn: Makine öğrenimi algoritmaları için.

Çalışmanın görseline erişmek isterseniz:

https://github.com/selcenbilek/Career-_HuBT-Veri-_Bilimi-_E-itimi/blob/main/Lineer%20Regresyon%20Modeli.png


