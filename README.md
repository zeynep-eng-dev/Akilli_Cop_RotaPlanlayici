<div align="center">

<!-- GRADIENT BANNER ALANI -->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 360" width="100%" style="border-radius: 12px; box-shadow: 0 12px 28px rgba(0,0,0,0.4);">
  <defs>
    <linearGradient id="bgGradient" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#1e1b4b" />
      <stop offset="50%" stop-color="#311b92" />
      <stop offset="100%" stop-color="#0f172a" />
    </linearGradient>
    <linearGradient id="textGradient" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#38bdf8" />
      <stop offset="50%" stop-color="#818cf8" />
      <stop offset="100%" stop-color="#c084fc" />
    </linearGradient>
  </defs>

  <!-- Arka Plan -->
  <rect width="100%" height="100%" fill="url(#bgGradient)" rx="12"/>

  <!-- Başlık Metinleri -->
  <text x="50%" y="85" text-anchor="middle" fill="url(#textGradient)" font-family="system-ui, -apple-system, sans-serif" font-weight="900" font-size="40" letter-spacing="1">Akıllı Çöp Toplama Rota Planlayıcı 🚛</text>
  <text x="50%" y="125" text-anchor="middle" fill="#94a3b8" font-family="system-ui, -apple-system, sans-serif" font-weight="500" font-size="18">Java &amp; Swing ile Geliştirilmiş Akıllı Rota Simülasyonu ☕</text>

  <!-- macOS Terminal Pencere Simülasyonu -->
  <g transform="translate(250, 155)">
    <!-- Terminal Kutusu -->
    <rect width="700" height="170" rx="10" fill="#090d16" stroke="#1e293b" stroke-width="2"/>
    
    <!-- macOS Pencere Düğmeleri -->
    <circle cx="22" cy="20" r="6" fill="#ef4444"/>
    <circle cx="42" cy="20" r="6" fill="#eab308"/>
    <circle cx="62" cy="20" r="6" fill="#22c55e"/>
    
    <!-- Terminal Kod Satırları -->
    <text x="22" y="55" fill="#38bdf8" font-family="Consolas, monospace" font-size="14" font-weight="bold">$ java AkilliCopRotaPlanlayici</text>
    <text x="22" y="82" fill="#e2e8f0" font-family="Consolas, monospace" font-size="13">[01] Parametreler Yüklendi: [Limit: 30kg] [Kapasite: 150kg] [Araç: 3]</text>
    <text x="22" y="107" fill="#e2e8f0" font-family="Consolas, monospace" font-size="13">[02] Konteynerler Sınıflandırıldı: 🟢 35% Hafif | 🟧 25% Orta | 🟥 40% Acil Dolu</text>
    <text x="22" y="132" fill="#4ade80" font-family="Consolas, monospace" font-size="13">[03] Rotalar Çizildi: Java Swing Harita GUI Başlatıldı! ✨</text>
  </g>
</svg>

<br/><br/>

[![Java](https://img.shields.io/badge/Language-Java_17+-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)](https://www.java.com)
[![GUI](https://img.shields.io/badge/GUI-Java_Swing-007396?style=for-the-badge&logo=java&logoColor=white)](https://docs.oracle.com/javase/tutorial/uiswing/)
[![Architecture](https://img.shields.io/badge/Architecture-OOP_%26_Modular-blueviolet?style=for-the-badge)]()
[![Status](https://img.shields.io/badge/Status-Aktif_Geliştirme-success?style=for-the-badge)]()

</div>

---

## 🎯 Proje Hakkında

Bu proje; şehir genelindeki çöp konteynerlerinin **koordinatlarını ($x, y$) ve anlık doluluk ağırlıklarını (kg)** analiz ederek, araç filolarının kapasitelerini en verimli şekilde yöneten ve en verimli toplama rotalarını çıkaran **Java tabanlı bir simülasyon sistemidir.**

---

## 🗺️ Nasıl Çalışır?

1. **Program Başlatılır:** Temel parametreler girilir.
2. **Parametre Girişi:** Çöp toplama limiti, araç kapasitesi ve araç sayısı belirlenir.
3. **Veri Kaynağı:** Konteyner bilgileri CSV dosyasından okunur *(dosya yoksa rastgele üretilir)*.
4. **Sınıflandırma:** Kutular ağırlıklarına göre **Hafif**, **Orta** ve **Dolu** olarak ayrılır.
5. **Dağıtım ve Rota:** Dolu kutular bölgelere ayrılır ve en kısa yol rotası çizilir.
6. **Görselleştirme:** Sonuçlar konsola yazdırılır ve Java Swing harita arayüzünde gösterilir.

---

## 🎨 Harita Gösterge Rehberi (Legend)

* 🟢 **Hafif Kutular** *(Toplama pas geçilir)*
* 🟧 **Orta Kutular** *(Takip listesinde)*
* 🟥 **Dolu Kutular** *(ACİL! Rotaya dahil edilir)*
* ⬛ **Depo / Merkez** *(Başlangıç ve bitiş noktası)*
* 🚛 **Araç Rotaları** *(Canlı renkli çizgiler)*

---

## 📂 CSV Dosya Formatı

```csv
id,x,y,agirlik
1,10,20,35
2,30,15,12
3,40,40,48
4,20,35,25
