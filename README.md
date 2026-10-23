[Akıllı Çöp Toplama Rota Planlayıcı](BURAYA_GITHUB_BANNER_LINKI) ([image](BURAYA_RAW_BANNER_LINKI))

# 🚛 Akıllı Çöp Toplama Rota Planlayıcı

Java ile geliştirdiğim bir rota planlama projesi. Çöp kutularının konum ve doluluk bilgilerine göre hangi kutuların toplanması gerektiğini belirliyor, kutuları araçlara dağıtıyor ve araçlar için rota oluşturuyor.

## 🗺️ Nasıl Çalışır?

1. Program çalıştırılır.
2. Çöp toplama limiti ve araç kapasitesi girilir.
3. Kullanılacak araç sayısı belirlenir.
4. Çöp kutularının bulunduğu CSV dosyası programa verilir.
5. Kutular doluluk durumlarına göre **Hafif, Orta ve Dolu** olarak sınıflandırılır.
6. Dolu kutular araçlara bölgelere göre dağıtılır.
7. Her araç için ayrı bir toplama rotası oluşturulur.
8. Sonuçlar konsolda gösterilir ve harita üzerinde görselleştirilir.

## 🗺️ Harita

Program Java Swing kullanarak çöp kutularını ve araç rotalarını harita üzerinde gösterir.

- 🟢 Hafif kutular
- 🟠 Orta dolulukta kutular
- 🔴 Dolu kutular
- ⬛ Depo
- 🚛 Araç rotaları

## 📂 CSV Dosyası

Çöp kutuları `id,x,y,agirlik` formatındaki CSV dosyasından okunur.

Örnek:

```csv
id,x,y,agirlik
1,10,20,35
2,30,15,12
3,40,40,48
4,20,35,25
```

CSV dosyası verilmezse program rastgele çöp kutuları oluşturabilir.

## ▶️ Çalıştırma

```bash
javac AkilliCopRotaPlanlayici.java
java AkilliCopRotaPlanlayici
```

Program sırasıyla toplama limiti, araç kapasitesi, araç sayısı ve CSV dosya adını ister.

## 📚 Bu Projede Kullanılanlar

- `Java`
- `Java Swing`
- `Scanner`
- `CSV` dosyası okuma
- `ArrayList`
- `Random`
- `Math`
- `if / else`
- `for / while`
- Rota planlama
- Grafiksel harita gösterimi

## 🚀 Gelecek Planları

- Daha gelişmiş rota optimizasyonu
- Gerçek harita verileri kullanmak
- GPS verisi eklemek
- Gerçek zamanlı çöp kutusu verileri kullanmak
- Araçların gerçek zamanlı konumlarını göstermek
- Farklı rota algoritmaları eklemek

## 👤 Geliştirici

Java ve algoritma öğrenme yolculuğumda geliştirdiğim bir rota planlama projesi. ☕🚛
