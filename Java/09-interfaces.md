- by default methods in interfaces are by default "public abstract"
- interface is not a class
- if methods of not defined, it will become abstract
```java
   interface A{
       void show();
       void pause();
   }

   class B implements A{
   // both the methods  must be defined
   }
   ```
- variables are final and static inside interfaces, it means we have to initialize the variables

```java

interface A
{
	int age=44;            // final and static 
	String area="Mumbai";
	
	void show();
	void config();
}

interface X
{
	void run();
}
interface Y extends X
{
	
}

class B implements A,Y
{
	public void show(){System.out.println("in show");}
	public void config(){System.out.println("in cofing");}
	public void run(){System.out.println("running...");}
}

public class Demo {
    public static void main(String[] args) {

    	A obj;
    	obj=new B();
    	
    	obj.show();
    	obj.config();
    	
    	X obj1=new B(); // refernce of X, obj of B
    	obj1.run();
    	
 //   	A.area="Hyderabad"; // error
    	
    	System.out.println(A.area); // pawsible
        
    }
}

```
