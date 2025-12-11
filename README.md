# genetik_optimizasyonu
## Proje Amacı ve Tanıtımı

Bu proje, Genetik Algoritma (GA) kullanarak kısıtlı bir optimizasyon problemi olan maksimum enerji verimi (y) hedefine ulaşmayı amaçlamaktadır.

---

### Öğrenci ve Proje Bilgileri

* Öğrenci Adı Soyadı: Rümeysa Canpolat
* Okul Numarası: 2312721021
* GitHub Repo Bağlantısı: [https://github.com/rum3ysa/genetik_optimizasyonu]

### Problemin Modeli

Amaç Fonksiyonu:
$y = 6x_{1} + 4x_{2} - 0.1x_{1}^{2}$ (Enerji Verim Puanı)

Kısıtlar ve Değişkenler:
1. $x_{1}$ (Eğim Açısı): 10° ile 45° arası olmalı.
2. $x_{2}$ (Sapma Açısı): 0° ile 90° arası olmalı.
3. $x_{1} + 0.5x_{2} \le 60$ (Alan Sınırı)
4. $x_{2} \ge 15$ (Minimum Yönlenme)

### GA Çözüm Sonuçları

Algoritma, 100 nesillik çalışma sonucunda kısıtları ihlal etmeden en yüksek verim puanını bulmuştur.

* Optimal Eğim Açısı ($x_{1}$): 17.94°
* Optimal Sapma Açısı ($x_{2}$): 84.07°
* Maksimum Enerji Verim Puanı ($y$): 411.76
* Kısıt Kontrolü: $x_{1} + 0.5x_{2} = 59.98$ (Sınırda başarı.)

#### Analiz

Enerji Evrimi grafiği, çözümün 20-30. nesillerde kararlı hale geldiğini gösterir. Ceza mekanizması sayesinde, algoritma kısıt sınırını (60) zorlayarak 59.98 değerine ulaşmış ve bu sayede maksimum verim hedefine ulaşmıştır.

### Görselleştirmeler

Aşağıdaki grafikler, algoritmanın ilerleyişini ve çözümün kalitesini görsel olarak desteklemektedir.

1. *Enerji Verim Puanının Nesiller Boyunca Evrimi*
   ![Enerji Verim Puanının Nesiller Boyunca Evrimi](images/fitness_convergence.png)

2. *$x_{1}$ ve $x_{2}$ Değişkenlerinin Nesiller Boyunca Evrimi*
   ![x1 ve x2 Değişkenlerinin Nesiller Boyunca Evrimi](images/variables_evolution.png)
