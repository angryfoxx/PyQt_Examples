# PyQt Examples
Bu repo PyQt ile yaptığım mini projeler için açılmıştır.<br>
Elimden geldiğince örnekler eklemeye çalışacağım.

## Prerequisites
---
```
Python 3.x.x
PyQt5
requests
```
```bash
pip install -r requirements.txt
```

## Currency Converter
---
![](https://i.hizliresim.com/lfdbepo.png)
<br><br>
Anlık olarak Dövizlerinizi dönüştüreceğiniz bir uygulama. <br>
Döviz Kurları için kullandığım API -> [Frankfurter](https://www.frankfurter.app)
<br>
Avrupa Merkez Bankası tarafından yayınlanan döviz referans oranlarını takip eder. Veriler her günü saat 16.00 civarında yenilenir. 

### Kullanım
---
Hangi dövizler arası dönüşüm yapacaksanız seçip miktarı giriniz. 

#### Veri Kaydetme
---
Son çevirdiğiniz veriyi kaydetmenizi sağlar. <br>
 *Dosya > Verinizi Kaydedin...*  diyerek kaydedebilirsiniz veya *Ctrl + S* kısayolu ile de verinizi kaydedebilirsiniz. <br><br>
Örnek:

```
Amerikan Doları ----------> Türk Lirası
1 tane Amerikan Doları  =  9.7402 tane Türk Lirası
Tarih: 18.12  |  09.11.2021
```

#### Kurları Kaydetme
---
Programın içindeki bütün dövizlerin birbirleri arasındaki kurları kaydetmenizi sağlar.<br> 
*Dosya > Kurları Kaydedin...*  diyerek kaydedebilirsiniz veya *Ctrl + Shift + S* kısayolu ile de verinizi kaydedebilirsiniz. <br><br>
Örnek:

```
Türk Lirası -- Amerikan Doları = 0.10267
Türk Lirası -- Avustralya Doları = 0.13851
Türk Lirası -- Kanada Doları = 0.12778
Türk Lirası -- İsviçre Frangı = 0.09391
Türk Lirası -- Çin Yuanı = 0.65656
Türk Lirası -- Euro = 0.08867
Türk Lirası -- İngiliz Sterlini = 0.07579
Türk Lirası -- Hong Kong Doları = 0.79955
Türk Lirası -- Japon Yeni = 11.641
Türk Lirası -- Norveç Kronu = 0.87554
Türk Lirası -- Rus Rublesi = 7.3292
Türk Lirası -- İsveç Kronu = 0.88301

Tarih: 18.12  |  09.11.2021
```

## Password Generator
---
![](https://i.hizliresim.com/np8hz6c.png)
<br><br>
Çözülmesi imkansıza yakın parolalar oluşturmanızı sağlayan bir generator.<br> Tabloda da gördüğümüz gibi basamak sayısı arttıkça; sayı, küçük harf, büyük harf <br>ve noktalama işareti ekledikçe çözülme zorluğu gittikçe artıyor. <br><br>
<img src="https://i.hizliresim.com/nwtyr7k.png" width=425 height=425>

### Kullanım
---
Varsayılan ayarlarda *Generate* butonuna bastığınız zaman 5 bloktan oluşan ve her blok arasında kısa çizgi (-) olan bir şifre oluşturuyor. <br>
İstediğiniz veya istemediğiniz harf, sayı ve noktalama işaretlerini değiştirmek için kutucukların içine istediğinizi ekleyebilir ya da  silebilirsiniz. <br><br>
Blok sayısını arttırmak için aşağıda bulunan (statusbar'da) kutucuğun içine blok sayınızı girerek blokları artırabilir veya azaltabilirsiniz.<br>
Varsayılan ayarlara getirmek için *Sıfırla* butonuna basmanız yeterlidir. <br><br>

## Mail Sender
---
![](https://i.hizliresim.com/1s2kdgi.png)<br><br>
SMTP protokolü kullanarak mail gönderebileceğiniz bir uygulama. Sadece e-posta yollamak için kullanılan bu protokolde, basitçe, istemci bilgisayar SMTP sunucusuna bağlanarak gerekli kimlik bilgilerini gönderir, sunucunun onay vermesi halinde gerekli e-postayı sunucuya iletir ve bağlantıyı sonlandırır. <br><br>
![](https://i.hizliresim.com/5u5uhuf.png)<br>
### Kullanım
---
![](https://i.hizliresim.com/5ppm804.png) <br>
Açılan pencereden gönderim yapacağınız mail adresinizi girin.<br>
Yeni açılan pencereden sırasıyla kime, konu ve içeriği yazdıktan sonra gönderin.

#### Yeni Mail
---
Yeni bir sayfa açmak için *Dosya > Yeni* ya da *Ctrl + N*'yi kullanabilirsiniz.

#### Mail to .txt
---
Gönderdiğiniz maili .txt olarak kaydetmek için *Dosya > Kaydet* ya da *Ctrl + S*'yi kullanabilirsiniz.<br><br>Örnek:

```
Gönderen:    FromMailForPyQt@gmail.com
Alıcı:	ToMailForPyQt@gmail.com
Tarih:	18.12  |  09.11.2021
Konu:	PyQt5_Examples

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
```

#### Görünüm
---
Yazı boyutlarını ayarlamak için *Görünüm*'e tıklayın.
Büyütmek için *Yakınlaştır* veya *Ctrl + Artı* . Küçültmek için *Uzaklaştır* veya *Ctrl + Eksi* . Sıfırlamak için *Varsayılan yakınlaştırmayı geri yükle* veya *Ctrl + 0*'a basarak boyutları isteğinize göre değiştirebilirsiniz.

## Installing
---
Klasör dizininde komut penceresini açıp "python exchange.py" | "python send_mail.py" | "python generator.py" komutunu girdikten sonra program başlayacaktır.

## Notes
---
**Currency converter Kurları Kaydetme:** 33 döviz birimi olduğu için ( 33 * 32 = 1056 tane ) işlemi yapması biraz uzun sürebilir.<br><br>

**Password generator:** Varsayılan ayarlarda her blok için '84240' farklı ihtimal bulunur. Varsayılan ayarlarda  bir şifre için de ihtimal sayısı 421200'dür. ( Blok sayısı 5 olarak alınmıştır. )<br><br>

**Mail Sender:** Eğer mail adresiniz bilinmeyen uygulamaların kullanımına kapalıysa [buradan](https://myaccount.google.com/lesssecureapps) erişimi açarak kullanmalısınız. 

## Authors
---
* **Ömer Faruk Korkmaz** - [angryfoxx](https://github.com/angryfoxx)

## License
---
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details