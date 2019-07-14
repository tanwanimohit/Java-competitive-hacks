# Java-competitive-hacks

This Article is for competitive coders who are looking to start coding in java. Will cover almost each and every hack ! and you can always add suggest new trick/hack via pull request. Let's get started.....

## Important Libraries 

```
import java.io.*;
import java.util.*;
```
 ## To Take Input in java 
 
 - Buffered Reader (Recommended)
 > Always returns String. you can easily convert into other type using parse syntax
 ```
BufferedReader br=new BufferedReader(new InputStreamReader(System.in));
br.readLine()
 ```
 - Scanner Class 
 ```
Scanner sc=new Scanner(System.in);
sc.nextInt(); //Replace Int with any other premitive data type.
sc.nextLine(); //To read Strings.
 ```
 
## Big Integer Class in java 
> There are many built in Math functions, which will make our work easy.

**Library**
```
import java.math.*;
```

Basic Syntax 
```
BigInteger bi= new Big Integer("String which contains Integer(s)");
```
Functions 
```
bi.multiply(bigintegervar)
bi.Add()  //This will Return Value BI is Immutable 
divide() 
pow() 
shiftLeft() 
shiftRight()
flipbit()
bitLength()
bitCount()
bi.valueOf()
bi.isProbablePrime(1) //to check the Prime.
bi.nextProbablePrime()
bi.Equals(bi2)
bi.compareTo(bi2)
bi.abs() //Absolute Value.
```


