## Java vs C++ Strings
##### Memory Management:
Java: Managed by JVM, stored in heap, immutable.
<br>
C++: Managed manually or with STL, mutable or immutable.

##### Null-Termination:
Java: Not null-terminated, objects with methods.
<br>
C++: Null-terminated (C-style) or managed internally.

##### Standard Library Support:
Java: Rich methods in java.lang.String class.
<br>
C++: std::string class in STL, extensive methods.

##### Concatenation:
Java: + operator or concat() method, immutable. Moves to next address
<br>
C++: + operator, append() method, mutable.

##### Unicode Support:
Java: UTF-16 encoding, native support for Unicode.
<br>
C++: No built-in support, but std::wstring for wide characters.

## Immutable String in Java
Whenever a change to a String is made, an entirely new String is created. 
<br>
However, java provides multiple classes through which strings can be used. 
<br>
Two such classes are StringBuffer and StringBuilder. 
##### StringBuffer:
```
  StringBuffer str  = new StringBuffer("Hello");
```
Thread-Safe: StringBuffer is synchronized, making it safe for multi-threaded environments.
<br>
Performance: Slightly slower due to synchronization overhead.
<br>
Mutability: Mutable - contents can be modified after creation.
<br>
Introduced: Since Java 1.0.
##### StringBuilder:
```
   StringBuilder str   = new StringBuilder("Hello"); 
```
Not Thread-Safe: StringBuilder is not synchronized, optimized for single-threaded scenarios.
<br>
Performance: Faster than StringBuffer due to lack of synchronization.
<br>
Mutability: Also mutable, allows modifications.
<br>
Introduced: Since Java 5.0.


