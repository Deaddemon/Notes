- Status is a class here.
- Enum class cannot be extended
```java
enum Status{ 
	Running, Failed, Pending, Success; // these are objects
}

public class Demo {
    public static void main(String[] args) {

    	int i=5;
     	Status s= Status.Running;

    	
    	System.out.println(s);
    	System.out.println(s.ordinal());
    	
    	Status[] ss=Status.values();
    	System.out.println(ss);
    	
        
    }
}
```
```java
enum Laptop{

	Mackbook(2000), XPS(2200), Surface, ThinkPad(1800);
	
	private int price;
	
	private Laptop()
	{
		price=500;
	}
	
	private Laptop(int price)
	{
		this.price=price;
	}
}
```
