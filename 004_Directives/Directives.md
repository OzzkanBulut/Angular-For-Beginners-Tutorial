## Directive Nedir?
* HTML elemanlarına ekstra özellikler ve davranışlar eklemek için kullanılan özel etiketlerdir.
* Bir başka deyişle DOM nesnelerini manipüle etmemizi sağlayan özel yapılardır.
* Angular'da davranışlarına göre farklı işlevsellik gösteren hazır directiveler mecvuttur.Bunların dışında kendimize özel directiveler de oluşturabiliriz.

## Directive Nasıl Kullanılır ?
![image](https://github.com/OzzkanBulut/Angular-For-Beginners-Tutorial/assets/67637654/aacdd260-578f-430d-beb4-3b931ef3753c)
* HTML elemnına directive ile hedeflenen davranışı kazandırabilmek için directive'ın selectorının buraya bildirilmesi yeterlidir.
* Bildirilen directive'ın davranışı her ne ise ilgili HTML elemanı bundan etkilenecek ve bu davranış sonucuna göre şekilleniyor/manipüle ediliyor olacaktır.

## Built-in/Hazır/Ön Tanımlı Directive'ler Nelerdir?
* Custom directive'leri geliştirmeden önce mimari tarafından bizlere sunulan ve belirli işlemlere odaklı davranışlar sergileyen directive'leri incelemekte fayda vardır. Bu directiveler şunlardır:
  - ngFor
  - ngSwitch
  - ngIf
  - ngClass
  - ngStyle
  - ngModel
  - NgNonBindable

## ngFor Directive
* HTML nesneleri üzerinde iterasyonel işlemler yapmak için kullanılan directivedir.
![image](https://github.com/OzzkanBulut/Angular-For-Beginners-Tutorial/assets/67637654/2abe8a45-e536-49e7-b387-8b191f3cd824)
* Verilen array/veri kümesi içerisindeki eleman sayısı kadar ilgili HTML nesnesini repeat edecektir.
* Ayrıca istendiği taktirde aşağıdaki gibi kullanılarak her bir elemanın index değeri de elde edilebilir.
![image](https://github.com/OzzkanBulut/Angular-For-Beginners-Tutorial/assets/67637654/cceee860-9d85-4db3-9bc7-987f8fa19023)
* Veya index,first,last,even ve odd keywordleri eşliğinde ngFor directiveini daha da karmaşık şekilde kullanabilirsiniz.

 ## ngIf Directive
* Verilen koşula göre HTML nesnelerinin görünürlüğünü kontrol etmek için kullaanılan temel bir Angular directiveidir.
![image](https://github.com/OzzkanBulut/Angular-For-Beginners-Tutorial/assets/67637654/0a2fd1ca-3df7-4c35-85f1-456f4d99f1f2)
* if/else mantığında işlev yapabilmek için aşağıdaki gibi de kullanılabilir:
![image](https://github.com/OzzkanBulut/Angular-For-Beginners-Tutorial/assets/67637654/f840f583-6b17-43ae-9845-bc782ad14839)
* ngIf directiveinde else/if mantığında davranış doğrudan sergilenememektedir. Bunun yerine ilgili mantıkta şöyle bir pratik çözüm uygulanabilir:
![image](https://github.com/OzzkanBulut/Angular-For-Beginners-Tutorial/assets/67637654/6bfd1dd1-173a-42fc-b9fe-48352cf11cb7)

## ngSwitch Directive
* Verilen koşula göre HTML nesnelerinin görünürlüğünü veya içeriğini değiştirmek için kullanılan temel bir directivedir.
![image](https://github.com/OzzkanBulut/Angular-For-Beginners-Tutorial/assets/67637654/762d9520-a899-47a3-8e27-f393666f1416)
* Görüldüğü üzere ngSwitch directive'i, ngSwitchCase ve ngSwitchDefault directiveleriyle birlikte kullanılmaktadır.

## ngClass Directive
* HTML etiketlerinin class değerlerini dinamik olarak yönetebilmemizi sağlayan directive'dir.
![image](https://github.com/OzzkanBulut/Angular-For-Beginners-Tutorial/assets/67637654/b8bddac4-2a8b-4555-a8bd-5fd364a71c82)

## ngStyle Directive
* HTML etiketlerinin style değerlerini dinamik olarak yönetebilmemizi sağlayan directive'dir.
* ![image](https://github.com/OzzkanBulut/Angular-For-Beginners-Tutorial/assets/67637654/ed383b4f-3060-474e-9bdb-05a0de71be1e)

## ngModel
* Form uygulamalarında kullanılan ve two-way data binding yapmamızı sağlayan bir directivedir.

## ngNonBindable
* Text Interpolation işlemini geçersiz kılan ve metni olduğu gibi renderlamaya yarayan directive'dir.



 
 





