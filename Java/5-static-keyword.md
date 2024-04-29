### static variables
```.java
public class Example { 
    static int count = 0;

    static{
        count = 1;
        System.out.println(count + "in static block");

    }

    // Method to display the count
    public static void displayCount() {
        System.out.println("Count: " + count);
    }

    public static void main(String[] args) {
        // Creating objects/refernce variables of Example class
        Example obj1 = new Example();
        Example obj2 = new Example();
        Example obj3 = new Example();

        obj1.count = 5; // not preferred, as static varibles must be called with class name.
        Example.count = 4 ; // will get changed for all objects 
    }
}


```

### static method
cannot use non-static variable inside static method
<br>
can use if we have object reference
```.java

Example.displayCount(Obj1); // accordingly parameters will also change for the method

```


### "main" method
Without static
<br>
first we will have to create object of Demo
<br>
then only main method will be able to invoke
```.java
public class Demo{
  public void main(String a[]){

}
}
```

But with static 
<br>
we can directly call main method
```.java
public class Demo{
  public static void main(String a[]){

}
}
```


### static block
called only once
<br>
inside class loader
<br>
calling a class without creating object
```.java
Class.forName(className: "Example");
```

