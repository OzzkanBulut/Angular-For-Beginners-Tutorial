## Modules
* Angular mimarisinde module yapılanması uygulama öğelerinin gruplandırılmasını sağlamaktadır.
Böylece uygulama daha düzenli bir şekilde inşa edilebilir hale getirilmektedir.
* Modüller, uygulamanın çeşitli parçalarını(components,services vs.) bir araya getirerek
  bir bütün olarak kullanılabilir kılmaktadır.
* Modüller birbirlerini import etmedikleri taktirde, bir modüldeki parça diğer modül altındaki parçalar
  tarafından erişilemez.
* Ayrıca modüller Dependency Injection pattern'ı kullanarak uygulamadaki öğeler arasında bağımlılıkları yönetmekte ve böylece test edilebilirlik ve bakım açısından kolaylık sağlamaktadırlar.
* Modüller ayrıca, Angular'ın işlemleri optimize etmek için kullandığı "Lazy Loading" özelliğini de destekleyerek sadece ihtiyaç duyulduğu taktirde yüklenmelerini de sağlayabilmektedirler.
