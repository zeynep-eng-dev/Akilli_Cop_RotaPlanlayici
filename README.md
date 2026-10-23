<div align="center">

# 🚛 Akıllı Çöp Toplama Rota Planlayıcı
### *Java ile Geliştirilmiş Akıllı Rota ve Konteyner Yönetim Sistemi*

[![Java](https://img.shields.io/badge/Language-Java-orange?style=for-the-badge&logo=openjdk&logoColor=white)](https://www.java.com)
[![Swing](https://img.shields.io/badge/GUI-Java%20Swing-blue?style=for-the-badge)](https://docs.oracle.com/javase/tutorial/uiswing/)
[![Status](https://img.shields.io/badge/Status-Aktif%20Geliştirme-success?style=for-the-badge)]()

</div>

---

## 📌 Proje Hakkında
Bu proje; çöp kutularının konum ve doluluk oranlarını analiz ederek hangi kutuların toplanması gerektiğine karar veren, bu kutuları araçlara paylaştıran ve en verimli toplama rotalarını oluşturan kapsamlı bir **Java konsol ve GUI** uygulamasıdır.

---

## 🗺️ Nasıl Çalışır?

1. **Başlangıç:** Program çalıştırılır ve temel parametreler girilir.
2. **Parametre Girişi:** Çöp toplama limiti, araç kapasitesi ve kullanılacak araç sayısı belirlenir.
3. **Veri Kaynağı:** Çöp kutularının bilgileri CSV dosyasından okunur *(dosya verilmezse sistem rastgele kutu üretebilir)*.
4. **Sınıflandırma:** Kutular doluluk oranlarına göre **Hafif**, **Orta** ve **Dolu** olarak kategorize edilir.
5. **Dağıtım ve Rota:** Dolu kutular bölgelerine göre araçlara atanır ve her araç için özel rota çıkarılır.
6. **Görselleştirme:** Sonuçlar hem konsola yazdırılır hem de Java Swing tabanlı arayüzde harita üzerinde çizdirilir.

---

## 🎨 Harita Gösterge Rehberi (Legend)

Java Swing arayüzünde kullanılan renk kodları:

* 🟢 **Hafif Kutular**
* 🟠 **Orta Dolulukta Kutular**
* 🔴 **Dolu Kutular**
* ⬛ **Depo (Merkez)**
* 🚛 **Araç Rotaları**

---

## 📂 CSV Dosya Formatı

Çöp kutusu verileri `id,x,y,agirlik` formatında okunur.

**Örnek `kutu_verileri.csv`:**
```csv
id,x,y,agirlik
1,10,20,35
2,30,15,12
3,40,40,48
4,20,35,25
