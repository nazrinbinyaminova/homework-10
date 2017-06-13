# Object Oriented ve diger paradigmalar
1. Emrlerin icra edilmesi novune gore asagindaki proqramlasdirma paradigmalari var:
    * imperative paradigma:
       * bu paradigmada emrler yeni emeliyyatlar ardicilliqla yerine yetirilir. Xaricden tesir edile biler.
    * functional paradigma:
       * xarici tesirleri olur
    * declarative paradigma:
       * emeliyyatin nece yerine yetirilidiyi vacib olmur, esas emeliyyatin yerine yetirilmesidir
    * object-oriented paradigma:
       * her seye bir obyekt kimi baxilir ve bu obyektlerin ozlerine xas xususiyyetleri olur. Obyektler bir sinif altinda birlesir. Object-oriented paradigmasinda bir classda olan deyisiklikler diger classlara, obyektlere tesir gostermir, yalniz o class daxilinde kecerlidir.
Bu xususiyyetlerine gore men object-oriented paradigmasini ozume yaxin gorurem, cunki burda bir-birinden asili olmayan hisselerle islemek mumkundur.
2. OOP paradigmasinda obyektler bir-birinden asili olmayan classlarla isleyir. Obyektlerin ozlerine mexsus olan xususiyyetleri bir classda saxlanilir ve obyekt daxil ederken bu classdan istifade edilir. OOP bize imkan yaradir ki, bir obyektlerde her hansi bir emeliyyat deyisdirende ve ya elave edende class vasitesile hemin classa aid olan butun obyetlerde bu emeliyyat icra edilsin. Bu diger classlara tesir gostermeyecekdir. OPP vasitesile hem de biz ferqli classlarda eyni adla deyisen goture bilerik. Bu deyisenler bir-birine qarismir, cunki hemin classdan xaricde islemir. Diger paradigmalarda ise bu mumkun deyil. Meselen:
```
public class Person
{
    public string Name { get; set; }
    public int Age { get; set; }
    public Person(string name, int age)
    {
        Name = name;
        Age = age;
    }
    //Other properties, methods, events...
}
```
Bu kodda ilk once `Nazrin` ucun `name` deyiseni, yaddasi ayrilir, sonra ise yeniden `name` deyisenine `Gunel` menimsedilir.

```
var name=Nazrin;
var name=Gunel;
```
3. OOP-nin 4 esas konsepti var:
    * Abstraction - 
    * Polymorphism - 
    * Encapsulation - 
    * Inheritance - 