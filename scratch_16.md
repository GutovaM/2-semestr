### Task 1 (8kyu)
Square(n) Sum

Complete the square sum function so that it squares each number pas sed into it and then sums the results together.
### Solution
```java
public class Kata
 {
  public static int squareSum(int[] n)
  { 
   int i = 0;
   int result = 0;
    while(i < n.length){
      //int i1 = Math.pow(i,2);
      result += Math.pow(n[i],2);
      i++;
    }
    return result;
  }
 }  
```
### Favourite
```java
import java.util.Arrays;

public class Kata {
  public static int squareSum(int[] xs) {
    return Arrays.stream(xs).map(x -> x * x).sum();
  }
}
```
[Task link](https://www.codewars.com/kata/515e271a311df0350d00000f)
### Task 2 (8kyu)
Century From Year

The first century spans from the year 1 up to and including the year 100, the second century - from the year 101 up to and including the year 200, etc.
### Solution
```java
public class Solution {
  public static int century(int number) {
    int n1 = number / 100;
    int n2 = number % 100;
    int result = 0;
    if(n2 > 0){
      result = n1 + 1;
      }
    else if(n2 == 0){
      result = n1;
      }
  return result;
  }
}        
```
### Favourite
```java
public class Solution {
  public static int century(int number) {
    return (number + 99) / 100;
  }
}
```
[Task link](https://www.codewars.com/kata/5a3fe3dde1ce0e8ed6000097)
