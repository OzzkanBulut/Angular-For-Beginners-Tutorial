## Modules
* Angular mimarisinde module yapılanması uygulama öğelerinin gruplandırılmasını sağlamaktadır.
Böylece uygulama daha düzenli bir şekilde inşa edilebilir hale getirilmektedir.
* Modüller, uygulamanın çeşitli parçalarını(components,services vs.) bir araya getirerek
  bir bütün olarak kullanılabilir kılmaktadır.
* Modüller birbirlerini import etmedikleri taktirde, bir modüldeki parça diğer modül altındaki parçalar
  tarafından erişilemez.
* Ayrıca modüller Dependency Injection pattern'ı kullanarak uygulamadaki öğeler arasında bağımlılıkları yönetmekte ve böylece test edilebilirlik ve bakım açısından kolaylık sağlamaktadırlar.
* Modüller ayrıca, Angular'ın işlemleri optimize etmek için kullandığı "Lazy Loading" özelliğini de destekleyerek sadece ihtiyaç duyulduğu taktirde yüklenmelerini de sağlayabilmektedirler.

## Components
* Component'ler uygulamanın görüntüleme katmanını ifade eden ve veri modeliyle etkileşim kurarak kullanıcılara uygulamanın görsel kısmını sunan yapılardır.
* Yapısal olarak birer HTML ve TypeScript dosyalarından oluşmaktadır.
* Uygulamanın bütün işlevsel operasyonlarının temel merkezini ifade eder.
* Sayfanın ta kendisidir. Kullanıcıların yapacağı bütün aksiyonları alacak ve bu aksiyona göre gerekli business çalışmasını yönetecek öğedir.
* Componentler, veri modeliyle etkileşim kurabilmek için **Data Binding** özelliğini kullanmaktadırlar.
* Ayrıca ihtiyaç duydukları servislerin instancelarını Dependency Injection ile elde edebilirler.
* Ortalama bir Angular uygulaması, birbirlerirle etkileşimli bir dizi component barındırarak dinamik ve etkileşimli işlevsevllik gösterebilmektedir.

## Data Binding
* Angular mimarisi, Data binding özelliği sayesinde veri modeli ile template'ler arasında veri kaışını dinamik bir şekilde sağlayabilmektedir.
* Böylece uygulamadaki verisel değişiklikler otomatik olarak sayfalara yansıtılabilmektedir.
* Angular'da Data Binding çift yönlü çalışmaktadır(Two Way Data Binding). Yani veri modeli güncellendiği zaman template'te, template güncellendiği zaman ise veri modeline anında yansıtılmaktadır.

## Dependency Injection
* Angular mimarisi, uygulamada mevcut olan öğeler arasındaki bağımlılıkları yönetebilmek için Dependency Injection pattern'ını kullanmaktadır.

## Directives
* Directive'ler, HTML nesnelerinin davranışlraını ve görünümlerini yönetebilmemizi sağlayan özel etiketlerdir.
* Angular uygulamalarını olabildiğince automatize etmemizi sağlar.
* Directive'ler, Angular'ın güçlü özellikleridirler ve uygulamanın oldukça dinamik ve etkileşimli olmasını sağlamaktadırlar.

## Decorators
* Decorator'lar, TypeScript dilinin bir özelliğidir ve angular tarafından kullanılmaktadır.
* Decorator sayesinde bir class'a yahut herhangi bir class member'ına -metadata- ekleyebilmekteyiz. Böylece ilgili yapının davranışı hakkında bir öntanımda bulunmaktayız.
* Misal olarak, bir class'ı @Component decorator'ı ile işaretlersek bir component, yok eğer @Injectable ile işaretlersek bir servis olacağı anlamına gelmektedir.

## Services
* Angular'da genellikle dış servislerle(API-endpoint) iletişim kurmak, karmaşık iş operasyonlarını veya business logic'i yürütmek yahut component'ler arasında iletişim sağlayabilmek için kullanılan fiili yapılanmalardır.
* Fiili bir yapının, işin sorumluluğunu üstlenmektedir. Okul servisi gibi düşün, seni okula getirip götürme sorumluluğunu üstlenir.
* Tüm operasyonel/fiili/kodlama gerektiren işlemler servislerde yapılmaktadır.

## Template
* Template, componentlerın HTML kısmıdır. İçerisinde HTML kodları barındırabileceği gibi özel angular elemanları, directive'ler, pipelar vs barındırabilir ve bunları işlevlerine göre çalıştırabilirler.
* Data Binding özelliğini desteklemekte ve böylece veri modeliyle dinamik bir şekilde etkileşime girebilmektedir.

## Guards
* Angular uygulamasında route erişimlerinin izin kontrolleri Guard yapılanması üzerinden gerçekleştirilmektedir.
* Sayfalar arası geçiş süreçlerinde ilgili kullanıcının erişimine izin verilip verilmeyeceğine dair karar veren yapılanmalardır.,
* Authorization işlemleri burada yönetilir.
* Angular uygulamasının güvenliği ve gizliliği Guard yapılanması tarafından üstlenilmektedir. Koruyucu gibi düşün

## Pipes
* Pipe'lar, verilerin görüntülenme süreçlerinde işlenmesine yönelik işlevsellik sağlayan yapılardır.
* Misal olarak, bir verinin tarihsel yahut parasal biçime dönüştürülmesi pipe'lar sayesinde gerçekleştirilebilir.
* Veriler üzerinde istediğimiz makyajı yapar
