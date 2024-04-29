```.java
// Java program to demonstrate reference
// variable in java
 
import java.io.*;
 
class Demo {
    int num = 5;
    public int add(int n1, int n2)
    {
        System.out.println("num = " + num);
        return n1+n2;
    }
}
 
class Main {
    public static void main(String[] args)
    {

          int data = 10;
          Calculator obj = new Calculator();
           Calculator obj1 = new Calculator();
          int r1 = obj.add(3, 4);
  
    }
}
```
![image](https://github.com/Deaddemon/Notes/assets/77224604/de2c2710-37af-47a6-86ae-80de4ff73282)

