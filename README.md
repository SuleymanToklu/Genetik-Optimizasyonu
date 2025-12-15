# Genetik Optimizasyonu ile Öğrenci Etüt Programı Planması

#### Bu proje Isparta Uygulamalı Bilimler Üniversitesi 3. Sınıf dersi olan Yapay Zeka Sistemleri dersinin 1. ödevidir. Amaç, belirli zaman kısıtlamalarına tabi olarak, Matematik ve Fen Bilimleri derslerine ayrılan çalışma saatlerine bağlı olarak başarı puanını en üst düzeye çıkarmaktır.

## Akış Şeması

<img width="2816" height="1536" alt="akisSemasiYZS" src="https://github.com/user-attachments/assets/e5f3bf0a-4fe9-4d6e-b86c-89e04b84ce25" /> 

## Problem Tespiti & Seneryo

**Seneryo:** Bir öğrenci, sınav başarısını en üst düzeye çıkarmak için çalışma saatlerini planlamak istiyor.
**Fonksiyon:** y = 4x₁ + 5x₂ - 0.5x₁² - 0.2x₂² (başarı skoru)
**Değişkenler:**
  o x₁: Matematik etüt süresi (saat) → [0, 10]
  o x₂: Fen etüt süresi (saat) → [0, 10]
**Kısıtlamalar:**
1.  Toplam çalışma süresi (Matematik ve Fen dersleri) 12 saati geçemez: x₁ + x₂ ≤ 12
2.  Fen Bilimleri dersi için minimum 2 saat ve üzeri çalışılmalı: x₂ ≥ 2

##  Özellikler
**Genetik Algoritma Uygulaması:** Seçim, çaprazlama ve mutasyonu içeren özel uygulama.  
**Kısıtlama Yönetimi:** Geçersiz çözümleri ele almak için kullanılan ceza yöntemi.  
**Görselleştirme:** Nesiller boyunca uygunluk evrimini gösteren Matplotlib grafiği.

## Sonuçların Yorumlanması ve Analiz

<img width="855" height="547" alt="sonuc" src="https://github.com/user-attachments/assets/31e6fcaa-e93d-4279-8890-b8f3e2d88e66" />


### Optimizasyon Sonucu

Matematik Süresi (x1) : 2.8918 saat -
Fen Süresi (x2)       : 9.1074 saat -
Toplam Süre           : 11.9992 saat 

Hesaplanan Başarı Puanı: 36.3340



Algoritma 100 jenerasyon sonunda **36.33** başarı puanına ulaşarak stabil hale gelmiştir.

Elde edilen değerler (Matematik Süresi (x₁): 2.8918 saat,  Fen Süresi (x₂): 9.1074 saat) incelendiğinde:
1.  **Kısıt Yönetimi:** Toplam süre 11.9992 saat olarak bulunmuş, 12 saat sınırına tam olarak dayanmıştır. Bu, algoritmanın elindeki kaynağı sonuna kadar kullanmaya çalıştığını gösterir.
2.  **Stratejik Dağılım:** Amaç fonksiyonunda Fen dersinin getirisinin (5x₂) Matematikten (4x₁) yüksek olması sebebiyle, algoritma Matematik süresini optimum tepe noktası olan 4 saatin altında tutarak (~2.89), kalan süreyi Fen dersine aktarmayı tercih etmiştir.
3.  **Başarı:** Algoritma, kısıtlar altında mümkün olan en yüksek skoru bulmak için "Matematik süresinden feragat etme" stratejisini başarıyla uygulamıştır.
