# Türkçe İsim Ekleri #

PHP 5.4 ve üzeri gerektirir. Ayrıca ***mbstring*** kurulu değilse çalışmayacaktır.


2015 yılında r10.net'teki bir tartışma üzerine yazıp, [şurada](https://www.r10.net/php/1440063-php-ekler-class.html) paylaşmıştım.

## Kullanabileceğiniz metotlar

 * birlikte
 * aitlik
 * yonelme
 * belirtme
 * bulunma
 * ayrilma

## Kullanımı

```
$ek = new Ekler('Emre'); 
// opsiyonel olarak iki değer alır. (string)isim ve (boolean)tırnak. 
// otomatik tırnak eklenmesini istemiyorşuradasanız false olarak girmelisiniz 

echo $ek->belirtme(); // Emre'yi 
echo $ek->isim("Sena")->yonelme(); // Sena'ya 
echo $ek->aitlik(); // Sena'nın 
echo $ek->isim('Ufuk', false)->ayrilma(); // Ufuktan

```

## Lisans
[MIT](/LICENSE)
