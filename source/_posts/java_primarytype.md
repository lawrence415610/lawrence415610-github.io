---
title: Java_primarytype 
tags: Java 
date: 2023-09-05 08:08:00
---

```java
// 1 bit information is 0 or 1, patterns number: 2**1, n bits yields 2**n patterns
byte b = 5; // 8 bits -128 to 127
short s = 128; // 16 bits -32768 to 32767
int i = 40000; // 32 bits (around 2 billion)
long l = 2222222222l; // 64 bits (more than 2 billion)

float f = 4.0f; // 32 bits
double d = 67.0; // 64 bits
BigDecimal number = new BigDecimal("3.4343434"); // to create accurate floating number, you need to use a class called BigDecimal, and pass the value as a string, it's immutable, should used as an Object
number.add(new BigDecimal(i)); // if you need to add, you should use method, and convert other type to bigdecimal
char ch = 'a';
```

In Jshell, you can check the size by calling
```java
Byte.SIZE
Byte.BYTES
Byte.MAX_VALUE
```

The number starts with a 0 is Octal, for example
```java
int eight = 010; // int eight = 8;
```
The number starts with a 0x is hexadecimal, for example
```java
int sixteen = 0x10; // int sixteen = 16;
```

Char can be used to present unicode charactor, for example
```java
char ch = '\u8DD1'; // 跑
```


- Question: What are the default values for object member variables when they are not explicitly initialized?
Answer: null for reference types, and 0 for primitive types
