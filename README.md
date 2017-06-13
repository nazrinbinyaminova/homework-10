# Object-oriented ve diger paradigmalar
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

```
var name=Nazrin;
var name=Gunel;
```
Bu kodda ilk once `Nazrin` ucun `name` deyiseni, yaddasi ayrilir, sonra ise yeniden `name` deyisenine `Gunel` menimsedilir.

3. OOP-nin 4 esas konsepti var:
    * Abstraction - proqramci qarisiqliq yaranmasin deye obyektin xususiyyetlerini gizledir, yalniz hemin classin icerisinde hemin xususiyyetler kecerlidir.
    * Polymorphism - bir deyisenin, bir funksiyanin, bir classin muxtelif mena ve ya meqsedler ucun istifade edilmesi. Numune:
```
public class Shape
{
    // A few example members
    public int X { get; private set; }
    public int Y { get; private set; }
    public int Height { get; set; }
    public int Width { get; set; }
   
    // Virtual method
    public virtual void Draw()
    {
        Console.WriteLine("Performing base class drawing tasks");
    }
}

class Circle : Shape
{
    public override void Draw()
    {
        // Code to draw a circle...
        Console.WriteLine("Drawing a circle");
        base.Draw();
    }
}
class Rectangle : Shape
{
    public override void Draw()
    {
        // Code to draw a rectangle...
        Console.WriteLine("Drawing a rectangle");
        base.Draw();
    }
}
class Triangle : Shape
{
    public override void Draw()
    {
        // Code to draw a triangle...
        Console.WriteLine("Drawing a triangle");
        base.Draw();
    }
}
```

   * Encapsulation - kapsullama,gizleme demekdir. Bir sinfin daxilinde olan obyektin xususiyyetini almaga icaze vermeyen bir gizleme novudur. `public` - aciqdir, kodun her hansi bir yerinde istifade edile biler. `private` - gizlidir, yalnizca hemin class daxilinde isledile biler.`protected` - gizlidir, sinif ve ya toreme sinifde istifade edile biler. `internal` - bir tertib daxilinde kodlarda istifade edile biler.
   * Inheritance - Miras vermek, varislik bir classin davranislarini goturub, genislendirib ve deyisdirerek yeni bir classin yaradilmasidir. Esas class (valideyn) alan ise toreme class (ovlad) adlanir.Toreme class yalniz bir valideyne sahib ola biler.
4. Class obyektlerin xususiyyetlerini ozunde birlesdirir.