

``` The `super()` method is used in object-oriented programming languages like Java and C++ to call a constructor in the parent class ```

``` `this()` will call constructor of same class```

``` Object is a class in java, every class extends Object ```

1) Method overloading occurs when multiple methods in the same class have the same name but different parameters, while method overriding occurs when a subclass provides its own implementation of a method that is already defined in its superclasses. 


## final keyword
1) similar to const in c++
2) can be applied to varible, method, class(stops inheritance)
   
## access modifiers

![image](https://github.com/Deaddemon/Notes/assets/77224604/c1fe608a-3db2-4efb-8920-7780a938726e)


## no multiple inheritance in java
![image](https://github.com/Deaddemon/Notes/assets/77224604/0bfddbac-8b12-49b9-b531-d8d9535bad19)

## upcasting and downcasting
```java
class A{}
class B extens A{}

public class Demo{
   public static void main(String a[]){
         A obj = new B();  // upcasting
         B obj1 = (B) obj; // downcasting
   }
}
```

## packages 
``` whichever class you use in java, belongs to a package```
``` by default 'import java.lang.*;' is there. '*' means all files```
![image](https://github.com/Deaddemon/Notes/assets/77224604/2492d69c-b6d3-4e04-a739-49dcf8d33c34)
