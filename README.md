# UML CLASS DİYAGRAMLARI

### Uml nedir
Programlama dillerinden bağımsız bir şekilde tasarım yapma ve bunu görsel hale getirmek maksatlı kullanılna bir yöntemdir. UML(Unified Modeling Language) türlü amaçlarla kullanılabilir ve türlü uml tipleri vardır. Bu repoda oop dünyasında kullandığımız class diyagramlarını ele alacağım.

### Class Gösterimi
Oop paradigmasında en çok kullandığımız yapılar olan classların uml temsilleri aşağıdaki gibidir.
![uml](https://github.com/hasanbaysal/Uml-Class-Diagrams/blob/master/images/class-gosterimi.png)
### Erişim Belirleyicileri - Access modifiers
![uml](https://github.com/hasanbaysal/Uml-Class-Diagrams/blob/master/images/access-modifiers.png)

birinci görseldeki bulunan class temsilindeki işaretlerin anlamları yukarıdaki tabloda görünmektedir. Herhangi bir oop dil içerisindeki örnek olarak c# içerisindeki erişim belirleyicilerini karşılar 

### Uml İlişki Türleri - Uml Relationship Types
Class diyagramlarının nesneye yönelik programlama tasarımlarını açıklamak için kullanıldığından bahsetmiştik. Oop paradigması ile yazılım geliştirirken nesnelerin ve sınıfların birbirleri ile ilişki içerisinde olduklarını biliyoruz. hal böyleyken bu durum uml class diyagramları tarafından da çeşitli temsil şekilleriyle işlenir. Bu ilişkilerin türleri şu şekildedir.

![uml](https://github.com/hasanbaysal/Uml-Class-Diagrams/blob/master/images/uml-relationship-tpyes.png)

### Assocaition - Referans veya Birliktelik
Bir sınıf başka bir sınıf türünden nesne referansına sahip olabilir. Bu noktada aralarında bir assocaition olur yani ilişki. Bu ilişiki bu iki nesne veya sınıf arasında bir çizgi çizilerek gösterilir.

***Bu ilişki tek yönlüyse yani sadece bir taraf diğerine ait bir referans tutuyor ise bu ilişkiyi bir ok çizerek gösteririz. Bu okun yönü referansı tutulan nesneye doğru olacaktır***

Mesela sipariş sınıfı müşteriye ait bir referans tutar çünkü siparişin hangi müşteriye ait olduğu bilinemelidir.\
**Sipariş =========> Müşteri**

![uml](https://github.com/hasanbaysal/Uml-Class-Diagrams/blob/master/images/assocaition.png)

### Aggregation - Barındırma, İçerme
Assocaition'ın özel bir halidir. Aslında kodsal manada bir farklılık yokdur. Bu ilişiki türü sınıf/nesne arasındaki ilişikinin boyutu hakkında bize fikir verir.

- parça bütün ilişikisi vardır 
- her aggregation aynı zamanda bir associationdır
- bu ilişki türünde parçalar ve bütünler birbirinden ayrı şekilde yaşayabilir

**Örnek olarak :**
Bilgisayar ve çevresel diğer donanımları düşünün. Monitör, yazıcı, klavye, fare, kulaklık bunların hepsi bize masaüstü bilgisayarı verebilir bir araya gelerek. Bu parçaları tek başına da ele alabiliriz. Parçalardan birinin nesnesel olarak hayatı bitince diğer parçalar bundan etkilenmiyor.

![uml](https://github.com/hasanbaysal/Uml-Class-Diagrams/blob/master/images/aggregation.png)

### Composition - Bağımlı iyelik ilişkisi
Bu ilişki de Assocaition'ın özel bir türüdür. Aggregation ile çok benziyor lakin buradaki fark nesnelerin tek başına bir anlam ifade etmemesidir. Bu ilişkide parçalar ve bütün birbiridnen bağımsız şekilde bulunmaz. 
![uml](https://github.com/hasanbaysal/Uml-Class-Diagrams/blob/master/images/COPM.png)

**Örnek olarak :**
Bir insanı bilgisayar ortamındaki bir nesne olarak ele alalım ve insanı meydana getiren organlarının ayrı birer parça olarak ele alalım. Doğal olarak bu parçalar arasındaki birlikte olma haliyle ortaya konulan ilişki aslında insan sınıfndan oluşna insan nesnesini bir araya getirir. Bu parçaların kendi başlarıan bir anlamı yoktur. Sadece kalp tek başına bir anlam ifade etmez sağlıklı bir şekilde o organın çalışabilmesi için bir vucüt sisteminin içinde olması gerek. Yani parça ve bütün ayrı ayrı ele alınamaz. Agrregation ile arasındaki en büyük fark budur

![uml](https://github.com/hasanbaysal/Uml-Class-Diagrams/blob/master/images/farklar.png)




### Dependency - Bağımlılık  ilişkisi
Bir nesnenin başka bir nesneye bağımlı olması durumudur. Bağımlı olunan nesne üzerinde yapılan değişiklik. Bağımlılığın gerçekleştiği yerde değişimleri beraberinde zorunlu kılabilir. 
A sınıfı B sınıfına bağımlı ise A sınıfı  üst bir yapıdır B ise alt yapıdır. 

![uml](https://github.com/hasanbaysal/Uml-Class-Diagrams/blob/master/images/Dependency.png)

**USAGE İLİŞKİSİ** <br />

**Dependency ve usage birbirlerine benzer yapılardır. Dependency başka bir sınıfa daha çok field,propperty olarak daha çıplak bir şekidle bağımlılığı ifade ederken Usage daha çok geçici bir ilişkiyi temsil eder mesela A sınıfın B sınıfı method parametresi olarak kullanması durumu** <br />
Usage İlişkisi nesneler arasında çalışma zamanında şu şekillerde olabilir
- static değişken olarak
- method parametresi olarak başka bir nesneye ihtiyaç durumu
- local veya global kullanım şekilde

![uml](https://github.com/hasanbaysal/Uml-Class-Diagrams/blob/master/images/usage.png)


<br />


### Generallization/Inheritance - Kalıtım İlişkisi 

oop paradigmalarına aşinaysanız kalıtımın ne olduğunu ve ne kadar çok kullanıldığını biliyorsunuzdur. Bu ilişki türü aşağıdaki şekilde gösteririlir

![uml](https://github.com/hasanbaysal/Uml-Class-Diagrams/blob/master/images/kalıtım.png)



### Realization - Gerçekleşme İlişkisi 

İnterfacelerin implemente edilmesi durumunu ifade eden bu ilişki türü aşağıdaki şekildedir. Inheritance'ye benzerlik gösterir aradaki ilişki kesikli çizgilerledir. 

![uml](https://github.com/hasanbaysal/Uml-Class-Diagrams/blob/master/images/realization.webp)



### ÖRNEK BİR TASARIM DESENİ ÜZERİNDE UML DİYAGRAMI
iterator tasarım deseninin ifade ediliş biçimi
![uml](https://github.com/hasanbaysal/Uml-Class-Diagrams/blob/master/images/iteratorpattern1.png)



---------------------------
### KAYNAKLAR 

- [Kaynak 2](http://www.cs.sjsu.edu/~pearce/modules/lectures/uml/class/association)
- [Kaynak 3](https://tugrulbayrak.medium.com/uml-class-diyagramlari-4c3bb7e9cc4c)
- [kaynak 4](https://www.includekarabuk.com/kategoriler/genel/UML-Sinif-Diyagrami-Iliskileri.php#Dependency)
- [kaynak 5](https://www.c-sharpcorner.com/UploadFile/ff2f08/association-aggregation-and-composition/)
- [Kaynak 6 kod örnekleriyle](https://medium.com/@ibrahimyengue/association-aggregation-and-composition-in-c-8cbeaa81201d)
