## **The homework repository of the 109. Innovance React Bootcamp by Kodluyoruz**

# **HOMEWORK 1**

### EFT Uygulaması

Bir banka uygulaması geliştirdiğımizi hayal edelim, bizim sorumlu olduğumuz kısma gelene kadar kullanıcı çoktan giriş yapmış ilgili menüden para transferi seçeneğini seçmiş olsun. 
Bizim geliştirmemiz gereken kısımda kullanıcı parayı gönderen hesabı kendi hesapları arasından seçiyor ve paranın gönderileceği hesabın IBAN'ını yazıyor olsun.
Ekranda olması gerekenler;
1) Dropdown (parayı gönderecek hesap - bakiye)
2) Textbox (para gönderilecek IBAN)
3) Numeric box (para miktarı)
3) Gönder butonu
4) Zaman sayacı (saniye cinsinden, 2 dakikadan geri sayar.)

Gereksinimler;
1) Kullanıcı parayı gönderen hesabı ve paranın gönderileceği hesabı seçmeden gönder butonu aktif olmamalı.
2) Kullanıcı gönderilecek para miktarına bakiyesinden daha çok yazamamalı, yazarsa gönder butonu aktif olmamalı ve ekranda hata olmalı.
3) Göndere basıldığı zaman miktar 500'den az ise kullanıcıya "Başarılı" geri bildirimi verilmeli.
4) Göndere basıldığı zaman miktar 500 veya daha çok ise kullanıcıya "Telefonunuza gelen şifreyi girin" sorusunu soran, 4 karakter numeric input yazabileceği bir UI çıkmalı.
5) Şifre girme esnasında 1234 girilirse ve enter'a basılırsa "Başarılı" geri bildirimi verilmeli.
6) Şifre 1234 değilse "Şifre yanlış" geri bildirimi verilmeli, 3 kere yanlış şifre girilirse 4.sünde "Hesabınız bloke oldu" geri bildirimi verilmeli
7) Herhangi bir işlem esnasında 2 dakikalik geri sayım süresi dolarsa kullanıcıya "Oturumunuz sonlanmıştır" geri bildirimi verilmeli ve sayfa yenilenmeli.

Notlar: geri bildirim vermek yada cep şifresi almak için alert/prompt metodları kullanılabileceği gibi tamamen özel bir UI'da yapılabilir. Burası size kalmış.
Kullanıcının bilgileri, hesapları ve bakiye bilgilerini user_information.js dosyası içerisinden kullanın.

# **HOMEWORK 2**


### Yemek Arama Motoru

Bir yemek arama moturu yapmakla sorumlusunuz, ana ekranda sadece bir arama kutusu ve login olan kullanicinin adı olacak. 
Kullanici veri girdikce bir arama yapacaksiniz ve cikan sonuclari listeleyeceksiniz.
Cikan sonuclar bir kartta listelenir. Kartın uzerine tıkladığınizda o karta odaklanacak. (Border olabilir ,ekranın ortasına gelebilir.). Kartta favorilere ekle butonu vardır. Kart açıkkan F tuşu ile ya da butona basarak favoriye/ekle çıkar işlemi gerçekleştirilebilir. Browser'i kapatip actiktan sonra da favorilerim kalmaya devam etmeli.


- Login olan kullanıcı bilgileri endpoint: https://jsonplaceholder.typicode.com/users/1
- Tüm yemek listesi endpoint: https://jsonplaceholder.typicode.com/todos (title, yemek adı olsun)
- Uygulama açıldığında kullanıcı bilgileri ve yemek listesi yüklenecek. Bu iki yükleme olurken ekranda loading  çıkacak.
- Login olan kullanıci bilgisi arama kutusunun ustunde Merhaba, {name} seklinde yazacak.
+ Arama yaparken fuse.js kullanmayı deneyin
+ Ard arda arama yaparken olabildiğince performanslı yazmayı deneyin. (Neler yapılabilir?)



# **HOMEWORK 3**


### Ülke Listesi / Istatistikleri Uygulaması

- Lütfen bu uygulamanızı React kullanarak yapın.
- Bu uygulamada Create-React-App kullanarak bir başlangıç yapın.

## Uygulama detayı

- Açılış sayfasında [Ülke Listesi, Istatistikler] adında iki buton olmalı. Ulke listesi ise açılışta seçili olarak gelmeli. (Tab gibi düşünebilirsiniz.)


- Ülke listesi seçili olduğu zaman ekranda API'dan dönen ülkelerin [Isim, Bayrak, Baskent, Dil] bilgilerinin yer aldığı bir kart olacak.

- Istatistikler seçili olduğu zaman ise ekranda bu ülkelerde en çok konuşulan 10 dil aşağıdaki formatta yer alacak.
    ```
    1) Dil Adı - Konusulan ulke sayisi
    ...
    10) Dil Adı - Konusulan ulke sayisi


    Orn: 
    1) English - 91
    2) French  - 45
    ```

- Olsa iyi olur: Uygulamanızi bir link üzerinden yayınlamayı  deneyin (deploy). Yayınlayabilirseniz readme dosyanıza live preview olarak o linki ekleyin. Kullanabileceğiniz örnek servisler: Vercel, Netlify (Başka yöntem kullanmakta özgürsünüz)


## API Link
https://restcountries.eu/rest/v2/all




# **HOMEWORK 4**

React mix example
Bu proje tamamen ReactJS kullanılarak yapılacaktır.
React'in Virtual DOM mantıgini bozmayan yardimci kutuphane kullanabilirsiniz. (Kesinlikle JQuery gibi DOM'a direk mudahale eden kutuphane kullanmak yasaktır.)
Ne istiyoruz?

- Ekranda 500px X 500px boyutunda köşe renkleri olan bir alan (oyun tahtasi) oluşturun.

- Bir karakter component'i oluşturun. Bu karakter 20px x 20px bir kare de olabilir sizin göstermek istediginiz bir image da olabilir.

- Uygulama acildiginda karakterimiz bu oyun tahtasinda yukari, asagi, sag, sol ok tuslariyla hareket edebilsin istiyoruz.

- Space tusuna basili tutulursa karakterin hareket etme hızı iki katına çıkmalı.

- Sayfa yenilenirse karakter kaldigi yerden devam etmeli.

- Karakter oyun tahtasindan cikamamali.

- Ekranda bulunan bir dropdown ile karakter degistirilebilir. Yani birden cok karakter componenti (en az 2) yapmanizi istiyorum.

- Uygulamayı tamamen React hooks ile yapmayı deneyin. Kendi hooklarinizi yazmakta cekinmeyin.

- Olabildigince duzenli kod yazmayi deneyin. Birden cok component olusturun.

- Istediginiz bir ESLint kuralini takip edin.

- Opsiyonel olarak uygulamanızı vercel, netlify v.b bir servise deploy edin ve linki readme dosyaniza ekleyin.

- Arkadaslarinizla discord uzerinden code-review yapin. En az 1 kere! Yazdiginiz kodlari karsilikli olarak nasil daha iyi hale getirebilirsiniz buna bakin.

- Daha iyi anlasilmasi icin ornek resimler. (Burada mario ve kare karakterleri yukari, asagi, sag, sol ok tuslariyla hareket edebiliyor. )


# **HOMEWORK 5**

## Chat APP


Birden çok odası bulunan, herkesin oda ekleyebildiği, herkesin anonim olarak herhangi bir odaya katılıp mesajlaşabildiği bir live chat app yapmanızı bekliyorum.
Çok temelde chat appimiz üç ekrandan oluşuyor.

1) Ana ekran (/login) ekranı

    -> Ekranda [Kullanici Adi] inputu ve [giris yap] butonu var.

    -> Herkes istediği username ile giriş yapabilir.

    -> Sifre sormaz, kayit mantigi yoktur. Herkes hizlica giris yapip mesajlasmaya baslayabilir.

2) Oda Listesi (/rooms) ekrani

    -> Giris sonrasi mevcut tum odalar listelenir. [Genel, GoyGoy, Teknoloji, ...] gibi odalar oluşturabilirsiniz.

    -> Bu ekranda istenirse yeni oda eklenebilir(Ekranin en altina bir yeni oda ekle butonu / input'u eklemek kafi.)

    -> Herhangi bir odanin uzerine gelindiginde odada kac kisi oldugu yazar ve chat'e katil butonu vardir.

3) Chat room (/room/room-name)

    -> Odaya katildiginiz zaman sol tarafta oda listesi gorunmeye devam eder. Sag tarafta bir chat kutusu ve chat gecmisi vardir. Anlik yazilanlar chat vasitasiyla gonderilir. Diger kisilerin ekranina anlik duser. (Discord gibi dusunun)


## Neler kullanalım
### React
### React-Router ya da ReachRouter
### Gerekiyorsa formik
### Realtime (canlı) chat ve database altyapısı için firebase yada seçeceğiniz servis.




 
 
 
 
 
 
# **GRADUATION PROJECT**

Bitirme projesi
Başvuru / ticket yönetim sistemi

Genel Açıklama
Uygulamamız herkese açık bir başvuru formunun son kullanıcı tarafından doldurulması ile başlıyor. Formu dolduran kullanıcıya başvurusunu takip edebilecegi bir kod veriliyor. Kullanıcı başvuru durumu sayfasından bu kod ile başvurusunun çözülüp çözülemedigini kontrol edebiliyor.

Kullanıcı adı ve şifre ile girilebilen bir ekrandan da yetkili kullanıcılar gelen başvuruları görüntüleyebiliyor cevaplanmamış başvurulara cevap yazıp durumunu çözüldü / iptal edildi / bekliyor vb gibi güncelleyebiliyor. Gerekirse eski kayıtlara ulaşabiliyor.

Detaylı Açıklama
Routes / Paths
/basvuru-olustur (default)

Public endpoint.
Başvuru formunu herhangi bir kullanıcının doldurmasına imkan verir.
Başvuru formunda [Ad, Soyad, Yaş, TC, Başvuru Nedeni, Adres Bilgisi, Fotograflar/Ekler, Gonder] butonu yer alır.
/basvuru-basarili (Basvuru formu doldurulduktan sonra gelen sayfa)

Ekranda bir teşekkür mesajı yer alır ve kullanıcıya başvuru detayları ile birlikte başvuru kodu verilir.
/basvuru-sorgula

Ekranda başvuru kodu girilebilen bir input ve sorgula butonu vardır.
/basvuru/{basvuruNo}

Ekranda başvuru varsa bilgileri, son durumu ve verilen cevap(lar) yer alır.
Başvuru numarası hatalıysa 404(bulunamadı) mesajı çıkar.
/admin

Ekranda kullanıcı giriş formu vardır. (Rahat test edebilmemiz için u:kodluyoruz, p:bootcamp109 bilgileri ile giriş yapabilmeliyim.)
/admin/basvuru-listesi

Başarıli giriş sonrası bekleyen (çözülmemiş/cevaplanmamış) başvuruların listesi yer alır ve basit bilgiler sunar. (Başvuru yapan, tarih)
Başvuru listesinde her elemenda başvuruyu görüntüle butonu vardır.
/admin/basvuru/{basvuruNo}

Başvurunun durumu güncellenebilir ve başvuruya cevap yazılabilir.
Burada yazılan cevap son kullanıci tarafından basvuru/{basvuruNo} kısmından görüntülenebilmelidir.

**Gereklilikler**
- React hooks
- Router (react-router/ reach router / etc)
- Context API
- Form management library (react-hook-form(önerilen) / formik / etc)
- Validation library (yup(önerilen), joi, etc)
- Tests (Unit test zorunlu, e2e opsiyonel)
- Uygulamanız kesinlikle bir servise deploy edilmiş olacak ve public link readme içinde yer alacak (netlify, vercel gibi)
- Open source
- Eslint

**Dikkat edelim**
- Tüm formlarda gerekli validasyonlar olsun.
- Back-end yazmak zorunda degilsiniz, back-end olarak firebase ya da mock bir api kullanabilirsiniz.
- Elinizden gelen en iyi şekilde seperation of concerns'e dikkat ederek yazın.
- Admin paneline u:kodluyoruz, p:bootcamp109 bilgileri ile giriş yapabilmeliyim.
- Mümkünse admin paneline bir menü ekleyelim (başvuru listesi, çıkıs gibi işlemleri kapsasın)
- Bonus (Zorunlu degil, deneysel ozellikler)
- Typescript
- Service worker ile offline render destegi
- Mobil uyumlulu guzel bir tasarim
- Kullanilabilir UX
