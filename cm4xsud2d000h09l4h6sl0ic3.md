---
title: "When doing a string comparison between the data entered and already set data."
datePublished: Sat Dec 21 2024 06:29:29 GMT+0000 (Coordinated Universal Time)
cuid: cm4xsud2d000h09l4h6sl0ic3
slug: when-doing-a-string-comparison-between-the-data-entered-and-already-set-data
tags: programming

---

Don’t use == as it will not work.

```java
import java.util.Scanner;
public class Integer{
  public static void main(String a[]){
    Scanner scanner = new Scanner(System.in);
    System.out.print("Username: ");
    String name = scanner.nextLine();
    
    if(name == "John"){ // it will not work
      System.out.println("Correct name");
    }
  
    scanner.close();
  }
}
```

So use the .equal() command to do that comparison

```java
import java.util.Scanner;
public class Integer{
  public static void main(String a[]){
    Scanner scanner = new Scanner(System.in);
    System.out.print("Username: ");
    String name = scanner.nextLine();
    
    if(name.equals("John")){
      System.out.println("Correct name");
    }
  
    scanner.close();
  }
}
```