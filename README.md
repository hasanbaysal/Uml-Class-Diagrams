# UML CLASS DİYAGRAMLARI

### Uml nedir
Programlama dillerinden bağımsız bir şekilde tasarım yapma ve bunu görsel hale getirmek maksatlı kullanılna bir yöntemdir. UML(Unified Modeling Language) türlü amaçlarla kullanılabilir ve türlü uml tipleri vardır. Bu repoda oop dünyasında kullandığımız class diyagramlarını ele alacağım.

### Class Gösterimi
![uml](https://github.com/hasanbaysal/Uml-Class-Diagrams/blob/master/images/class-gosterimi.png)
### Erişim Belirleyicileri - Access modifiers
![uml](https://github.com/hasanbaysal/Uml-Class-Diagrams/blob/master/images/access-modifiers.png)

birinci görseldeki bulunan class temsilindeki işaretlerin anlamları yukarıdaki tabloda görünmektedir. Herhangi bir oop dil içerisindeki örnek olarak c# içerisindeki erişim belirleyicilerini karşılar 

### Uml İlişki Türleri - Uml Relationship Types
Class diyagramlarının nesneye yönelik programlama tasarımlarını açıklamak için kullanıldığından bahsetmiştik. Oop paradigması ile yazılım geliştirirken nesnelerin ve sınıfların birbirleri ile ilişki içerisinde olduklarını biliyoruz. hal böyleyken bu durum uml class diyagramları tarafından da çeşitli temsil şekilleriyle işlenir. Bu ilişkilerin türleri şu şekildedir.

![uml](https://github.com/hasanbaysal/Uml-Class-Diagrams/blob/master/images/uml-relationship-tpyes.png)

### Assocaition - Referans veya Birliktelik
Bir sınıf başka bir sınıf türünden nesne referansına sahip olabilir. Bu noktada aralarında bir assocation olur yani ilişki. Bu ilişiki bu iki nesne veya sınıf arasında bir çizgi çizilerek gösterilir.

***Bu ilişki tek yönlüyse yani sadece bir taraf diğerine ait bir referans tutuyor ise bu ilişkiyi bir ok çizerek gösteririz. Bu okun yönü referansı tutulan nesneye doğru olacaktır***

Mesela sipariş sınıfı müşteriye ait bir referans tutar çünkü siparişin hangi müşteriye ait olduğu bilinemelidir.
**Sipariş =========> Müşteri**

![uml](https://github.com/hasanbaysal/Uml-Class-Diagrams/blob/master/images/assocaition.png)

### Assocaition - Referans veya Birliktelik