## Interpolation Syntax Nedir?
* Angular'da, Component Class'ı içerisindeki herhangi bir field veya property'nin değerini {{..}} operatörü aracılığıyla HTML içerisinde kullanılmasına Text Interpolation, bu ifadeye ise Interpolation Syntax denir.
* ![image](https://github.com/OzzkanBulut/Angular-For-Beginners-Tutorial/assets/67637654/5e80f9f4-9eb8-4ef3-a1e5-7c5fb3818e07)
* Interpolation, One-Way(Tek Yönlü) Data Binding gerçekleştirmektedir.
* Two-way binding yalnızca ngModule gibi form uygulamalarında gerçekleşir.

## Interpolation'da Neler Kullanılmaz ?
* Interpolation, yapısal olarak sadece field veya property değerlerini okumak ve böylece Template'e yansıtmak için kullanılır. Bundan dolayı uygulamanın durumunu(state) değiştirebilecek herhaangi bir işlem gerçekleştirememektedir.
* Bu mantıkla işlem neticesinde state değişikliğine sebebiyet verebilecek aşağıdaki operatörler,keywordler ve işlemler interpolation ile birlikte kullanılamaz:
   - Assign operatörleri(=, +=, -=)
   - new, typeof, instanceof vs. keywordleri
   - ; operatörü
   - Increment-Decrement operatorleri(++,--)
   - Bitwise Operatörler  
* Bunların dışında interpolation'da iki değişkeni aritmetik işleme tabi tutabilir, string birleştirme yapabilir, template referansı kullanabilir veya herhangi bir fonksiyonu tetikleyebilirsiniz.
![image](https://github.com/OzzkanBulut/Angular-For-Beginners-Tutorial/assets/67637654/96930195-ccb5-4218-906d-d1f1083b2a0b)
![image](https://github.com/OzzkanBulut/Angular-For-Beginners-Tutorial/assets/67637654/529c78c1-81e8-44ff-981b-e30983305ce4)

## Interpolation'da Script/HTML Kodları Çalıştırılabilir mi?
* Angular, Interpolation ile DOM' aekleyeceği içeriği her şeyden önce sterilize ederek Cross-Site Scripting Security Bugs(XXS) hatalarına karşı bir önlem alır. Bu yüzden interpolation ile gelen Script veya HTML kodları handle edilmeksizin oldukları gibi(metinsel olarak) yansıtılırlar.
* ![image](https://github.com/OzzkanBulut/Angular-For-Beginners-Tutorial/assets/67637654/4e5674a6-c0ae-42f4-8ff0-03304a33d515)

* ## NgNonBindable Nedir?
* * Interpolation operatörünün compile edilmesini istemediğiniz noktalarda bu özelliği aşağıdaki gibi devreye sokabilirsiniz:
   ![image](https://github.com/OzzkanBulut/Angular-For-Beginners-Tutorial/assets/67637654/13504a31-c338-40d3-83a6-e0d1e70da6f9)

## Extraadan Interpolation İle Kullanılan Operatörler
* Angular'da Interpolation ile ekstradan da aşağıdaki yapıları kullanabilirsiniz:
  - Pipes
  - Nullable operatörü (?)
  - Non-Null Assertion operatörü (!) --> Bu kesin null değil. Null olsa bile boşver sorumluluğu ben üstlenirim



