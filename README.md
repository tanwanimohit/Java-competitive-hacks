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

**Basic Syntax**
```
BigInteger bi= new Big Integer("String which contains Integer(s)");
```

**Functions**
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
[Lear more about Big Integer Class ](https://www.geeksforgeeks.org/biginteger-class-in-java/)

## Big Integer Usecases 

**Easily Check that Number is Prime or not :**
```
BigInteger bi = new BigInteger("1652")
bi.isProbablePrime(1) //This Will Return True Or False.
BigInteger.valueOf(1235) //Direct method
```

**Get Next Prime Easily :**
```
BigInteger bi= new BigInteger("5");
BigInteger b2=bi.nextProbablePrime(); //Return BigInteger
```

**Get GCD of Two Numbers Easily :**
```
BigInteger b1=new BigInteger("165");
BigInteger b2=new BigInteger("465");
BigInteger b3=b1.gcd(b2); //Return BigInteger
```

**ConvertTo Any Other Data Type :**
```
BigInteger bi=new BigInteger("5532");
int a=bi.intValue(); //Replace int with any other Data Type toString() is there as well !
// Side Note : For Comparing use compareTo() and equals() Functions.
```

**Work with Bits Easily :**
``` 
BigInteger bi=new BigInteger("5532");
int length=bi.bitLength() //to Get Length.
BigInteger changedvalue = flipBit(index) //to Flip the Bit at specific posssition in a number
BigInteger changedvalue = shiftLeft(n) //this<<n and shiftRight(n) this>>n For shifting Bits.
```

**Artihmatic Functions :**
```
BigInteger a=new BigInteger("10");
BigInteger b=new BigInteger("10");

//Addition
BigInteger c=a.add(b);

//Other Functions
multiply() //a*b
add() //a+b
divide() //a/b
subtract() //a-b
mod() //a%b
modInverse() //b%a
not() //!a
pow() //a**2 
and() //a&b
xor() //a^b
```

**For LCD in BigInteger :**
> Just Multiply Both the Numbers and divide that with GCD of Numbers (Use GCD Function).

## Other Tricks

**Quicky Convert to Binary/Octal/Hex:**
```
//use toString function of Integer
//Example: 

int n=1500;
String temp=Integer.toString(n,2) //here n is a variable of int and 2 is for Binary (8 for octal and 16 for hex)
//This will return string..

```

**If Else in System Out Print :**
```
System.out.println((a==0) ? "Yes it is" : "Nope! You are Wrong ");
	
// In Functions
return (x==0) //In Return Statements As well.
```

 **Different way of doing Multiplication and Division :**
```
int a =10;
a= a << 1; //Mutiply by 2
a= a >> 1; //Division By 2
```
 
 **Swapping using Xor:**
```
a ^= b;
b ^= a;
a ^= b;
```
 
 **To Find total Number of Digits Directly :**
 ```
int N=453;
int x=(int)Math.log(N)+1;
 ```
 
 **Quickly check whather no is power of 2 or not via function :**
```
 function checkPowerOf2(int n)
 {
     return (x!=0) && (x&(x-1)==0);
 }
```
 
 **For Each loop in java :**
 ```
for (int a: Arr_var)
{
	//Code.
}
 ```
 
 **Split the String Input using ShorCut method:**
 ```
 String strr[] = String/BufferedReader.readLine().split("AnyToken"); //As this will return String Array so no worries Just Acces that using index Like : sttr[0]

 ```
 
 **Convert String To CharArray:**
 ```
 char Arr[]= str.toCharArray();
 ```
 
 **String Replace:**
 ```
 str.replace("" , "");
 ```
 
 **Fill Array with a no.**
 ```
 int arr[]=new int[100];
 int value=15;
 Arrays.fill(arr,value);
 ```
 
 ## Sorting
 **Sorting Function:**
 ```
Arrays.sort(arr); //This Method uses QuickSort Algo !! 
//Complexity : O(nlogn);
 ``` 
 
 **Sort SubArray :**
 ```
 Arrays.sort(arr,starting,ending); 
 ```
 
 **Reverse Order Sorting:**
 ```
 Arrays.sort(arr,Collections.reverseOrder);
 ```
 
 ## Searching :
 
 **For Sorted Array use Binray Search :**
 ```
Arrays.binarySearch(arr,var_to_search);
ArraysbinarySearch(arr,start,end,var) //Within the Range..
 ```
 
 **String.indexof() function Usecases :**
>We Can search Character and string As wel in String.indexOf() Method and We can also Specify the Starting Element..
>We can also use this fucction on Substring Search..
```
//We Can search Character and string As wel in String.indexOf() Method and We can also Specify the Starting Element..
//We can also use this fucction on Substring Search..
 
String.index(char/String, Start_Var_int);

 ```
 
## Wrapper Classes :

Well, Wrapper classes have some inbuilt method, you can use it if you want to save your time I am just listing the Classes names you can [learn more about Wrapper classes here](https://www.tutorialspoint.com/java/java_numbers)
 

>int - Integer
>loat - Float 
>char - Character
>double- Double

## StringBuilder

**Basic Syntax**

```
Stringbuilder str=new Stringbuilder("String");

str.append("Mohit"); //Append String

str.insert(start,"Tanwani"); //Insert at Specific Location.

str.delete(start,end) //Delete from Specific Location.

str.reverse() //Reverse the String 

str.deleteCharAt(index) //Delete Character At Specific Location.
```

**IndexOf() in String**

```
str.indexOf("String") //To Get The Location of the SubString..
str.lastIndexOf() //last index of that Varaible.
```

**SubString In StringBuilder:**
```
str.substring(start,end);
```

**Replace Method:**
```
str.replace(start,end,"string");
```

**Substring And Store that into an array:**
```
char arr[] =new char[5];
str.getChar(start,end,arr,arrStart);
```

**SetCharAt():**
```
str.setCharAt(index,'M');
```

**Get unicode of the Letter:**
```
str.codePointAt(index);
```

**Convert to Normal String:**
```
String stt=str.toString();
```

## Output Trick With String Builder
> By using this trick you will save hell out of time.
Why ? Because `System.out.print()` Take too much time by this way we can reduce the time.
```
//Intialize this at the starting of the Program
StringBuilder str= new StringBuilder();

//Whenever you want to Print on screen just append that to String Builder object
str.append(Result).append('\n');

//and at the end print the Whole string...
System.out.println(str);
```

## Type Casting 
> Convert one data type to another.
**String to Integer**
```
int a=Integer.parseInt("1500");
```

**String to Float**
```
int a=Float.parseFloat("1500");
```

**To String datatype**
```
String abs=String.valueOf(int/float)
```

## Math Functions

```
Math.abs() //Absolute Value.
int x=Math.PI //PI value Inbuilt
Math.cbrt(No) //Cube Root of a number.
Math.log/log10() //Log of the Number.
Math.ciel();
Math.floor();
Math.sqrt() //Square Root
```


## Random Number Geneartion in Java

```
Random rn=new Random();
rn.nextFloat() //genrate Float Random Number
rn.new Int(); //genrate Int Random Number
rn.new Int(100); // Within Range
```
