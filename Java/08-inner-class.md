1) Outer class cannot be static
```java
class A
{
	int age;
	
	public void show()
	{
		System.out.println("in show");
	}
	
//	class B
//	{
//		public void config()
//		{
//			System.out.println("in config");
//		}
//	}
	
	static class B
	{
		public void config()
		{
			System.out.println("in config");
		}
	}
}


public class  Demo{
    public static void main(String[] args) {
    	A obj=new A();
    	obj.show();

    // in order to access B, we must have a obj of A first
    // A.B obj1=obj.new B();
    // obj1.config();

    // for static class
    	A.B obj1=new A.B();
    	obj1.config();

    }
}
```


## anonymus inner class
```java
class A
{
	int age;
	
	public void show()
	{
		System.out.println("in show");
	}

}


public class  Demo{
    public static void main(String[] args) {
    	A obj=new A(){

      public void show(){
      	System.out.println("Overrided, it is inside annonymus inner class");
        }

    };

obj.show(); // prints=Overrided, it is inside annonymus inner clas
    	

    }
}
```


## anonymus inner class and abstract class
```java
abstract class A
{
	public abstract void show();
	public abstract void config();

}


public class  Demo{
    public static void main(String[] args) {
    	
    	A obj=new A() 
    	{
    		public void show()
    		{
    			System.out.println("in new show");
    		}
    	};
    	obj.show();
    	
    }
}

```
