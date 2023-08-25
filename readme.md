Entegre Üretim Tesisi Sipariş Simulasyonu

## Senaryo
Bir fabrikada birden fazla üretim bandında birden fazla çeşit ürün işlenebilmektedir. 
Bu ürünler üretim bandının farklı noktalarından veya aynı noktalarından geçebilir.

### Bantlar
    -Giriş bandı
    -A bandı 
    -B bandı
    -C bandı
    -D bandı
    ...
    -Z bandı
    -Paketleme bandı
    -Çıkış bandı
    -Not: her bir bant aynı anda farklı sayıda ürün işleyebilir, her bir bantın birim işlemede "saatlik hızı" farklıdır. Örneğin saatte 10 ürün işleme hızına sahip bant eğer aynı anda 3 ürün işleyebiliyorsa, tüm ürünlerin aynı saatte banta girdiğini varsaydığımızda saatin sonunda 30 ürün işlemiş demektir.

### Ürün Çeşidi
    -Bir "ürün çeşidi" için hangi bantlardan geçeceğine dair bir yol tarifi oluşturulmalıdır.

### Yol Tarifi
    -Bir ürün çeşidi işleme alındığında hangi bantlardan geçeceğine dair sıra kaygısı güderek tarif listesi oluşturunuz.

### Ürünler
    -Bir ürün sadece 1 ürün çeşidine bağımlı olabilir.

### Siparişler
    -Bir sipariş listesi sistemi oluşturunuz.
    -Siparişte farklı ürünler, farklı sayılarda olabilir.
    -Siparişi işleme aldığınızda geçmiş siparişlerin üretim bandında harcayacağı süreyi de hesaba katarak siparişin muhtemel tamamlanma süresini hesaplayınız ve siparişe kaydediniz.
    -Bantlar neyi ne zaman işleyeceğini bir tablo vasıtasıyla bilmelidir.

### İstatistikler
    -Tamamlanmış siparişler için:
      -En uzun sürede tamamlanmış siparişleri listeleyiniz.
      -En çok kullanılan bantları listeleyiniz.
      -Herhangi bir bantta en çok hangi ürünler işlenmiş listeleyiniz.
      -Herhangi bir bantta belirlenen tarih aralığında kaç ürün işlenmiş listeleyiniz.

### Laravel Yetenek Beklentileri
-Tüm modeller için factory oluşturun. İlişkisel factory kullanımı + puan getirecektir.
-Tüm modeller için resource ve collection oluşturun. İlişkisel çağırımlar + puan getirecektir.
-Tüm modeller için doğru migration deklarasyonlarını yapınız. Foreign idlere dikkat ediniz.
-Tüm http post|put|delete işlemleri için Request classları oluşturunuz ve doğru kuralları uygulayınız. İhtiyacınız olan Rule'ları yeni class'lar açarak yazınız.
-Her bir model arasında "doğrudan" ilişki kurunuz ve methodlarını yazınız. (Doğrudan:Örneğin bir siparişe ait ürün çeşitlerini tek methodda listeleyiniz.)
-Gerekliyse modellerde scope, observer, ayrıca servis classları kullanınız.
