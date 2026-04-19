# 3.7 GHz Mikroşerit Yama Dizi Anten Tasarımı

## Proje Özeti
Sub-6 GHz 5G (n77/n78 bandı) haberleşme sistemleri için **3.7 GHz merkez frekansında çalışan mikroşerit yama dizi anten** tasarlandı, simüle edildi ve fiziksel olarak üretimi gerçekleştirildi.

Proje kapsamında:
- Simülasyonlar gerçekleştirilmiş,
- Anten performansı değerlendirilmiş, 
- PCB üretim süreci uygulanmış,
- Gerçek ölçüm sonuçları elde edilmiştir.

Bu yönüyle çalışma, **teorik + simülasyon + üretim** süreçlerini birlikte içermektedir.

## Kullanım Alanları
- 5G Baz İstasyonları (Sub-6 GHz)
- Sabit Kablosuz Erişim (FWA)
- İHA / Drone haberleşme sistemleri
- Endüstriyel kablosuz ağlar

## Kullanılan Teknolojiler
- **CST Studio Suite** (EM simülasyon)
- **FR-4 PCB** (εr ≈ 4.3, h = 1.6 mm)
- **Kimyasal aşındırma yöntemi**
- **SMA konnektör (50 Ohm)**

## Anten Tasarımı
- Çalışma frekansı: **3.7 GHz**
- Yapı: **4x1 mikroşerit yama dizi anten**
- Besleme: **Corporate feed**
- Empedans: **50 Ohm**
- Substrat: **FR-4**

<p align="center">
  <img src="https://github.com/user-attachments/assets/e72d95b7-b057-44c2-9be8-90dc020c90ae" width="45%" /><br>
  <em align="center">4x1 Anten Tasarımı</em>
</p>

## Sonuçlar

### Simülasyon Sonuçları

- S11: **3.7 GHz de -42 dB**
- Kazanç: **~9 dBi**
- Işıma: **Yönlü**

<p align="center">
  <img src="https://github.com/user-attachments/assets/f9cd7e23-31e8-4dab-b334-32612f282745" width="45%" /><br>
  <em align="center">Simülasyon S11 Grafiği</em>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/4ac928d9-bbbb-49f2-af9b-d2fbb4a9f65d" width="45%" /><br>
  <em align="center">Simülasyon Frafield Grafiği</em>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/d602c06d-d9d7-444f-ac13-df8a8729d761" width="25%" /><br>
  <em align="center">Simülasyon Kazanç/Işıma Deseni Grafiği</em>
</p>

### Ölçüm Sonuçları

- S11: **-29 dB @ 3.7 GHz**
- Frekans kayması: **Yok**

<p align="center">
  <img src="https://github.com/user-attachments/assets/27a2620e-95e2-41e7-859f-c73fade7ac2a" width="45%" /><br>
  <em align="center">Ölçüm Sonrası S11 Sonuçları</em>
</p>

Simülasyon ve ölçüm farklarının nedenleri:
- Üretim toleransları  
- Malzeme parametre sapmaları  
- Konnektör ve ölçüm kayıpları  

## Işıma Karakteristiği
- Ana lobda yoğun enerji yayılımı gözlemlenmiştir.  
- Yan loblar bastırılmış durumdadır. 
- Yönlü haberleşme için uygun bir yapı sunulmaktadır.

## Üretim Süreci

1. CST ortamında anten tasarımı  
2. Gerber çıktısının baskı devre kağıdına basılması  
3. Ütüleme yöntemi ile baskının PCB’ye aktarım  
4. Kimyasal aşındırma (H₂O₂ + HCl) işlemi 
5. Mürekkebin temizlenmesi   
6. SMA konnektörün lehimlenmesi

## Çalışma Prensibi
Anten, **corporate feed besleme ağı** kullanılarak RF sinyalini dizi elemanlarına eşit şekilde dağıtmak amaçlanmıştır. Bu ağ sayesinde,

- Faz uyumu sayesinde sinyaller üst üste biner  
- Belirli yönde yoğunlaşmış ışıma oluşur  
- Tekli antene göre daha yüksek kazanç elde edilir 

## Projenin Avantajları
- Yüksek kazanç ve yönlülüğe sahip olması. 
- Düşük maliyetli üretim (FR-4) yapılabilmesi. 
- Hafif ve kompakt yapıda olması. 
- RF sistemlere kolay entegre (50 Ohm uyumlu) edilebilir olması.

## Projenin Yapım Aşaması Görselleri

<p align="center">
  <img src="https://github.com/user-attachments/assets/c8b9388f-4dc2-4494-9af3-b08f2eca3502" width="25%" />
  <img src="https://github.com/user-attachments/assets/e58381cd-c587-4917-8f30-6b0062158702" width="35%" /><br>
  <em align="center">Bakıra Gerber Çıktısının Ütü İle Basılması ve Sonucu</em>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/ca95ea68-e520-4361-9ada-aaaa85b6ae6e" width="28%" />
  <img src="https://github.com/user-attachments/assets/32c12069-1029-479c-a31b-cf8090442d38" width="23%" /><br>
  <em align="center">Bakırın Eritilmesi ve Mürekkebin Çıkartılması</em>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/228dface-6966-452e-a3b1-5312b6fb6430" width="25%" /><br>
  <em align="center">SMA Lehimlenmiş Anten</em>
</p>

## Dokümantasyon
Detaylı rapora buradan ulaşabilirsiniz:
`docs/4x1_array_antenna_rapor.pdf`

## Çıkarımlar
- Simülasyon ve ölçüm sonuçlarının karşılaştırılması sonucunda, antenin hedeflenen 3.7 GHz merkez frekansta çalıştığı ve herhangi bir frekans kayması gözlenmediği doğrulanmıştır. Bu durum, tasarım sürecinde yapılan hesaplamaların ve optimizasyonların doğruluğunu ortaya koymaktadır.
- S11 parametresinin simülasyonda -42 dB, ölçümde ise -29 dB olarak elde edilmesi, antenin her iki durumda da oldukça iyi empedans uyumuna sahip olduğunu göstermektedir. Ölçümde gözlenen farkların üretim toleransları, malzeme özelliklerindeki sapmalar ve konnektör kayıplarından kaynaklandığı değerlendirilmiştir.
- Farfield analizleri, antenin yönlü bir ışıma karakteristiğine sahip olduğunu ve enerjinin büyük ölçüde ana lob yönünde yoğunlaştığını göstermektedir. Yan lob seviyelerinin düşük olması, istenmeyen yönlere yayılan enerjinin minimize edildiğini ve sistem verimliliğinin artırıldığını ortaya koymaktadır.
- Elde edilen sonuçlar, tasarlanan antenin 5G haberleşme sistemleri, sabit kablosuz erişim (FWA), drone haberleşmesi ve endüstriyel RF uygulamalarında kullanılabilecek potansiyele sahip olduğunu göstermektedir.







