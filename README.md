# Java ile PDF Özgeçmiş Oluşturucu

> Bu proje, Java ve iText 7 kütüphanesi kullanılarak programatik olarak profesyonel bir PDF özgeçmişi (CV) oluşturan bir komut satırı uygulamasıdır.

## 💻 Ekran Görüntüsü

Oluşturulan PDF dosyasının çıktısı aşağıdaki gibidir:

*(NOT: Bu ekran görüntüsünün projenizde görünmesi için, yüklediğiniz `Ekran görüntüsü_8-10-2025_192415_.jpeg` dosyasının adını daha basit bir şeye (örn: `ornek-cikti.jpeg`) değiştirip projenizin ana dizinine eklemeniz ve aşağıdaki satırı güncellemeniz önerilir.)*

![Proje Çıktısı](Ekran%20görüntüsü_8-10-2025_192415_.jpeg)

## 📝 Hakkında

Bu uygulama, herhangi bir grafik arayüze (GUI) ihtiyaç duymadan, doğrudan Java kodu içerisindeki verileri kullanarak düzenli ve modern bir CV oluşturur. Proje, iText 7 kütüphanesinin güçlü yerleşim (layout) özelliklerinden faydalanarak metinleri, görselleri ve diğer elementleri A4 sayfasına dinamik olarak yerleştirir. Kod, okunabilirliği artırmak ve bakımı kolaylaştırmak için yardımcı metotlar (helper methods) kullanılarak bölümlere ayrılmıştır.

## ✨ Özellikler

-   **Dinamik PDF Oluşturma:** Java kodu içindeki verileri anında PDF'e dönüştürür.
-   **Profesyonel ve Düzenli Tasarım:** Başlıklar, paragraflar, çizgiler ve kenar boşlukları ile okunaklı bir tasarım sunar.
-   **Görsel Ekleme:** Özgeçmişe kolayca profil fotoğrafı ekler.
-   **Kolayca Özelleştirilebilir İçerik:** Kod içindeki metinleri değiştirerek kendi özgeçmişinizi kolayca oluşturabilirsiniz.
-   **Maven ile Kolay Bağımlılık Yönetimi:** Proje, gerekli iText kütüphanesini Maven aracılığıyla otomatik olarak yönetir.

## 🛠️ Kullanılan Teknolojiler

-   **Java:** JDK 11
-   **Apache Maven:** Proje yönetimi ve bağımlılıklar için
-   **iText 7:** PDF oluşturma ve düzenleme kütüphanesi

## 📋 Gereksinimler

Projeyi çalıştırmak için sisteminizde aşağıdakilerin kurulu olması gerekmektedir:

-   Java Development Kit (JDK) 11 veya üstü
-   Apache Maven

## 🚀 Kurulum

1.  Projeyi klonlayın:
    ```sh
    git clone [PROJE_ADRESINIZ]
    ```
2.  Proje dizinine gidin:
    ```sh
    cd [PROJE_DIZINI]
    ```
3.  Maven, `pom.xml` dosyasındaki bağımlılıkları otomatik olarak indirecektir.

## ▶️ Kullanım

1.  Özgeçmişte kullanılacak profil fotoğrafını `src/main/Images/` dizini altına `Berathan.png` adıyla eklediğinizden emin olun.
2.  Projenin ana dizininde terminali açın ve aşağıdaki komutu çalıştırın:
    ```sh
    mvn clean compile exec:java
    ```
3.  İşlem başarılı olduğunda, `Düzenli PDF dosyası başarıyla oluşturuldu` mesajını göreceksiniz.
4.  Oluşturulan PDF dosyası, projenin ana dizinindeki `src/main/PDF-Dosya/ornek_duzenli.pdf` konumunda bulunacaktır.
