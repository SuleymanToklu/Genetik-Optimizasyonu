# Genetik Optimizasyonu ile Öğrenci Etüt Programı Planması

### Bu proje Isparta Uygulamalı Bilimler Üniversitesi 3. Sınıf dersi olan Yapay Zeka Sistemleri dersinin 1. ödevidir. Amaç, belirli zaman kısıtlamalarına tabi olarak, Matematik ve Fen Bilimleri derslerine ayrılan çalışma saatlerine bağlı olarak başarı puanını en üst düzeye çıkarmaktır.

## Akış Şeması

[ <img width="2816" height="1536" alt="akisSemasiYZS" src="https://github.com/user-attachments/assets/e5f3bf0a-4fe9-4d6e-b86c-89e04b84ce25" /> ]

## Problem Tespiti & Seneryo

**Seneryo:** Bir öğrenci, sınav başarısını en üst düzeye çıkarmak için çalışma saatlerini planlamak istiyor.

**Fonksiyon:** y = 4x₁ + 5x₂ - 0.5x₁² - 0.2x₂² (başarı skoru)

**Değişkenler:**
  o x₁: Matematik etüt süresi (saat) → [0, 10]
  o x₂: Fen etüt süresi (saat) → [0, 10]

**Kısıtlamalar:**
1.  Toplam çalışma süresi (Matematik ve Fen dersleri) 12 saati geçemez: x₁ + x₂ ≤ 12
2.  Fen Bilimleri dersi için minimum 2 saat ve üzeri çalışılmalı: x₂ ≥ 2

##  Özellikler * **Genetik Algoritma Uygulaması:** Seçim, çaprazlama ve mutasyonu içeren özel uygulama. * **Kısıtlama Yönetimi:** Geçersiz çözümleri ele almak için kullanılan ceza yöntemi. * **Görselleştirme:** Nesiller boyunca uygunluk evrimini gösteren Matplotlib grafiği.

##  Sonuçlar Algoritma, tüm kısıtlamaları karşılarken puanı en üst düzeye çıkaran en uygun çalışma sürelerine yakınsar. Ayrıntılı analiz not defterinde verilmiştir.
