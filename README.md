# Robomatik
İlkokullar için uzaktan kumandalı hesap makinesi. 4006 Tübitak Bilim Fuarı için yapılmıştır.

## Problem
Matematiğin küçük yaşlardan itibaren sevilmesi tüm öğretim hayatını olumlu etkiler.  Projemizin amacı anaokul ve ilkokul seviyesindeki öğrencilere matematiği severek öğrenmesini sağlamak için robotik ile birleştirerek yeni ve eğlenceli bir öğrenme metodu sunmak. 

## Araştırma Özeti
Matematiği sevdirmek üzere tasarlanmış mevcut uygulamalar, Arduino ile motor sürücü kontrolü, uzaktan aracı kontrol etmek için Arduino ile Bluetooth haberleşmesi, kamera ve OCR (Optik Karakter Tanıma) çözümleri, MIT App Inventor ile nasıl kolayca Android uygulaması geliştirileceği araştırıldı. Yapım için Arduino Uno, bir araç kiti, L298N motor sürücü, HC-05 Bluetooth modülü, ve ESP32-CAM kameralı mikrokontrolcü seçildi ve alındı.

## Gereksinimler
Projemizin üzerinde bulunan batarya ile çalışmalı, düşük maliyetli olmalı, görsel olarak aldığı basit problemleri önce yazı verisine dönüştürüp çözdükten sonra sesli olarak kullanıcıya doğru cevabı bildirmeli olduğuna karar verdik.

## Geliştirilen çözüm
Geliştirilen tasarımda elektriksel gücü bataryalar motor sürücüye, motor sürücü ise diğer bileşenlere gönderiyor. Motor sürücü ile Arduino arasındaki 4 pin hareket ettirilecek motorları, 2 pin ise bu motorların hızını kontrol ediyor. Uygulamadaki butonlardan birine basınca Bluetooth modülüne bir komut gönderiliyor, bu komut Arduino kodunda işleniyor ve uygun motor(lar) istenilen yönde çalıştırılıyor. Aynı uygulama ESP32’nin gördüğü görüntüyü çekiyor, Tesseract adlı OCR yazılımını kullanarak o görüntüden metni alıyor, matematik işlemini çözüyor ve sesli olarak cevabı söylüyor.

## Prototip
Bluetooth ve WiFi ile iletişim sağlayacak Android uygulaması, motor kontrolü ve Bluetooth iletişimi için Arduino üzerinde çalışacak yazılım, ve Kamera ve OCR için ESP32 üzerinde çalışacak yazılım geliştirildi. Tüm donanımların montajı yapılarak prototip hazır hale getirildi.

## Sonuç ve Değerlendirme
Çalışmalarımız neticesinde tasarımımızı prototip haline getirerek fikrimizin uygulanabilir olduğunu gördük. Tasarımımızın geliştirmeye açık olduğunu, ilkokul ve anaokul seviyesindeki öğrencilere matematiği eğlenceli hale getirebileceğini düşünüyoruz.

**Hazırlayanlar**
Tuna Tezer
Ege Erdem
Kartal Çakıcı
