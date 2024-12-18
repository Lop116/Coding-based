---
title: "You could either use an else or put a return outside the if statement"
datePublished: Wed Dec 18 2024 06:19:14 GMT+0000 (Coordinated Universal Time)
cuid: cm4ti5n4o000209lcf0au12np
slug: you-could-either-use-an-else-or-put-a-return-outside-the-if-statement
tags: programming

---

```java
public int division(int n1, int n2){
        if (n2 == 0 || n1 == 0){
            return 0;
        }
        else{
            return n1 / n2;
        }
    }
```

or you could use that, since if the condition are met, it will not go through the second return

```java
public int division(int n1, int n2){
        if (n2 == 0 || n1 == 0){
            return 0;
        }
        return n1 / n2;
    } 
```