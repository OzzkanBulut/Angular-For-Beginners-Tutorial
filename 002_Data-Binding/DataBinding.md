## Data Binding
![image](https://github.com/OzzkanBulut/Angular-For-Beginners-Tutorial/assets/67637654/7ec36c80-0de2-4f21-bc49-6def9bf9ee44)

## Binding Nedir ?
* Angularda Binding kavramı, Component Class'ında bulunan bir modelin vey afonksiyonun Template'deki bir lan yahut DOM nesnesi ile canlı bağlantı oluşturmasıdır.
* Binding, bağlantı yapısına göre aşağıdaki gibi şekillenebilmektedir:
  - Text Interpolations
  - Property Binding
  - Event Binding (Bu butona tıkladığında şunu yap)
  - Two Way Binding
  - Attribute Binding
  - Class Binding
  - Style Binding
  
## Text Interpolation
* Template içerisinde, Component Class'ı içerisinde tanımlı olan bir field/property değerinin yazdırılması için kullanılan Binding yöntemidir.
![image](https://github.com/OzzkanBulut/Angular-For-Beginners-Tutorial/assets/67637654/ca71a982-16f9-4f20-aa95-dfde12b977c0)

* Bu yöntemde, Component Clss'ındaki 'name' field'ı Template'teki ilgili alana bind edilmekte ve böylece 'name' üzerinde olabilecek tüm değişiklikler anlık olarak Template'teki alana yansıtılmış olacaktır.

## Property Binding
* Template içerisindeki HTML nesneleri veya directive'ler için Component Class'ında tanımlı olan verilerin property olarak direk bağlanmasını sağlayan yöntemdir.
* Şöyle ki:
![image](https://github.com/OzzkanBulut/Angular-For-Beginners-Tutorial/assets/67637654/c8378679-c5c0-48c3-be49-9de105a577c0)
* Bu yöntem sayesinde değer atamaları daha dinamik bir şekilde gerçekleştirilmiş olmaktadır.
* Ek olarak selector ile referans edilen componentlerin içerisindeki Input property'lere de Property Binding üzerinden görseldeki gibi değer atanabilmektedir:
![image](https://github.com/OzzkanBulut/Angular-For-Beginners-Tutorial/assets/67637654/c9ded234-8f1b-4fa5-ad5e-65f6662e10fe)

## Event Binding
* Template içerisindeki herhangi bir DOM nesnesinin, Component Classı içerisinde tanımlı olan bir fonksiyona event olarak bağlanmasıdır.
  ![image](https://github.com/OzzkanBulut/Angular-For-Beginners-Tutorial/assets/67637654/e0da8f10-22b8-4f2d-af73-c601cc15dcd9)
* Görüldüğü üzere Event Binding sürecinde DOM nesnesinde aksiyona göre tetiklenecek olay parantez içerisinde {event} şeklinde belirtilmektedir. Tabi burada isterseniz on-click şeklinde de olayı tanımlayabilirsiniz.
* İsterseniz event'lere karşılık tanımlanan fonksiyonları noktalı virgülle ayırarak da kullanabilirsiniz.
  ![image](https://github.com/OzzkanBulut/Angular-For-Beginners-Tutorial/assets/67637654/d77dd5fb-9fcf-4781-acea-55d7cf45f195)
* Bu işleme Multiple Event Handlers denmektedir.

## Two-Way Binding
* Template içerisindeki bir HTML nesnesinin değeri değiştiğinde, o nesneyle bind edilmiş olan Component Classı içerisindeki field/property değerinin nlık olarak değiştirilmesini ve aynı zamanda tam tersi durumunda geçerli olmasını sağlayan yöntemdir.
* Genellikle kullanıcıyla etkileşime giren form vb. uygulamalarda kullanılır.
* Html'de değişiklik yapan user, ts dosyasındaki değişkenin değerini de değiştirmiş olacaktır.
* View'da değişiklik olursa model'ı da değiştir.Model'da değişiklik olursa view'ı de değiştir!
* HTML nesneleri ile Two-Way Data Binding gerçekleştirebilmek için input nesnelerinde [(ngModel)] direktifi kullanılır.
* [(ngModel)] direktifini kullanabilmek için uygulamanın ana modülünde FormsModule'ün import edilmiş olması gerekmektedir.
* Ayrıca [(ngModel)] direktifi ile bind edilmiş olan bir HTML nesnesinde verisel değişiklik olduğu taktirde ngModelChange eventi ile bir olayı tetikleyebilir ve böylece girilen bilgilerin de doğrulanması için çalışma yapabilirisiniz.
* Tabi bir de HTML form elementleri için genel olarak kullanılan change eventi de mevcuttur. Bu event [(ngModel)] direktifi olmaksızın verisel değişikliklerde olay fırlatmak için kullanılabilir.
* Yani nalayacağınız ngModelChange, [(ngModel)] direktifi ile birlikte kullanılırken, change evet'i ise yalnız başına kullanılabilmektedir.

## Attribute Binding
* HTML elemanlarının attribute'lari için değerleri doğrudan Component Class'ından verilmesini sağlayan yöntemdir.
* Property binding ile aynı .
![image](https://github.com/OzzkanBulut/Angular-For-Beginners-Tutorial/assets/67637654/30dfa5dd-2f43-42e4-879a-d13735ca90f6)

## Style and Class Binding
* Bir HTML öğesine CSS ile ilgili style veya class bildirilerinde bulunmak için kullanılan yöntemdir.
![image](https://github.com/OzzkanBulut/Angular-For-Beginners-Tutorial/assets/67637654/5876305a-768a-443a-9a5a-a789398cc10e)

## Change Detection Algoritması
* Template'de bir event tetiklendiğinde veya kullanıcı eylemi sonucunda modelin verisi değiştiğinde Component Class'ı bilgilendirmek ve Template ile senkronizasyonu sağlayabilmek için Change Detection algoritması kullanılır.




