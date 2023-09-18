## Components
 * Angular uygulamalarında component'ler uygulamanın mühim parçası olan merkezi yapılanmalardan biridir
 * Genellikle angular uygulamasında component'lerin görevi sayfa altyapıları olarak kullanılmalarıdır. Bunun dışında sayfa olarak kullanılan componentlerin alt componentleri olarak da kullanılabilmekte ve böylece partial mantığında sayfaları geliştirmemize de imkan verebilmektedirler.
 * Her component, kendi işlevselliğine ve görünüme odaklıdır ve diğer component'lerden bğaımsız olarak çalışırlar.
 * Böylece, değiştirilmesi/onarılması/modifiye edilmesi gereken noktalar için sadece ilgili component üzerinde çalışmak yeterli olacaktır.
 * Böl,parçala,yönet!
 * Componentler, birbirleriyle iletişim kurarak, büyük ve karmaşık uygulamaları oluşturmayı kolaylaştırır.

## Component'in Bileşenleri Nelerdir ?
![image](https://github.com/OzzkanBulut/Angular-For-Beginners-Tutorial/assets/67637654/eb72346d-4b9c-46e3-b112-7b0286fe856f)

## Template
* Bir componentin görsel çalışmalarının yapıldığı parçasıdır.
* İçerisinde HTML kodunun eşliğinde directive ve pipe gibi özel Angular elemanları ve Data Binding davranışları kullanılabilmektedir.
* Component'in .html dosyasına karşılık gelmektedir ve component ile "templateUrl" field'ı üzerinden ilişkilendirilmektedir.
* Eğer ki template işlemlerini fiziksel olarak ayrı bir dosya üzerinden gerçekleştirmek istemiyorsnız direk .ts dosyası içerisinde "Template" field'ına karşılıkta çalışmalarınızı gerçekleştirebilirsiniz.

## Style
* Componentin css, scss vb. gibi artık hangi style türü seçildiyse ilgili çalışmalarının yapıldığı tasarım parçasıdır.
* .css .scss gibi türüne özgü uzantılı dosyalarına karşılık gelmektedir ve component ile "styleUrls" field'ı üzerinden ilişkilendirilmektedir.
* İstenildiği takdirte "styles" field'ı üzerinden de css'ler tanımlanabilmektedir. Template'de yaptığımız gibi aynı.
   
## Component Class
* Component'in merkezi ve esas unsurudur. Uzantısı .ts olan dosyadır.
* Tüm JavaScript, TypeScript ve jQuery işlemleri bu parça üzerinde gerçekleştirilir ve component içerisinde kullanılacak değişkenlerle birlikte fonksiyonlar bu sınıf üzerinde tanımlanır.
* Verileri nasıl görüntüleneceği, fonksiyonların nasıl işleneceği gibi işlevsellikler bu sınıf tarafından yönetilir.
* Uygulamada iş mantığı gereği, business logic barındıran servisler "Component Class" üzerinden çağırılırlar. Aynı şekilde API gibi dış servislere erişim sürecinin bşlatılmasından da bu sınıf sorumludur.

## Selector
* Component'in selector özelliği, ilgili component'in uygulamanın herhangi bir noktasında nasıl çağırılacağını tanımlayan bir referans özelliğidir.
* Sadece HTML dosyalarında kullanılabilir.
* <app-root></app-root>
* Uygulamadaki herhangi bir componentin HTML'inde farklı bir componentin selector'ı yukarıdaki gibi çağırılıyorsa eğer o selectore'a karşılık gelen component compiler tarafından render edilecek ve üretilen çıktısı o noktaya basılmış olacaktır.

## Metadata Decorator
* Componentin nasıl yapılandırılacağını ve nasıl kullanılacağını tanımlayan bir decoratordur.
* Bu decorator ile ilgili componentin, şu ana kadar gördüğümüz **selector**,**template**,**style** bilgileri eşliğinde componentler arası yönlendirme süreçlerindeki geçiş animasyonları[**animations**], componentin dışarıdan alabileceği değişkenler[**inputs**] yahut dışarıdan emitlenecek eventler[**outputs**] vs tanımlanabilir.
*  
