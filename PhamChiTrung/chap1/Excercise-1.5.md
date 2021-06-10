* Exercise 1.1.5
* Program 1

* a) The code is incorrect since the for loop should go from top to bottom, but it only goes from top to the element close to the bottom in this code, thus it can't provide a perfect answer.

```java
public static int findLast (int[] x, int y)
{ 
 
   for (int i=x.length-1; i >= 0; i--) 
   {
      if (x[i] == y) 
      {
         return i;
      }
   }
   return -1;
}
```
b ) 
If possible, give a test case that does not execute the fault.
test case
x=[7,9]
y=9
c )
If possible, give a test case that executes the fault, but does not result in an error state. 
x=[7,7]
y=7
d )
x = [1,0,3]
y= 1
* Program 2: Explain what is wrong with the given code. Describe the fault precisely by proposing a modification to the code.

```java
public static int lastZero (int[] x)
{ 
int index = -1
 for (int i = 0; i < x.length; i++)
{ 
 if (x[i] == 0)
{ 
 index = i;;
} 
}
 return index;
 }
```
* b
The missing initialization added before the loop is executed by all inputs.<br>
As a result, the defect is executed by all inputs

* Program 3<br>
a ) Describe the flaws in the provided code. Propose a code update to accurately describe the problem.<br>
we need to find positive element but in this code, we count 0, and 0 is not a positive number.

```java
public int countPositive (int[] x) 
{ 
int count = 0; 
for (int i=0; i < x.length; i++) 
{ 
if (x[i] > 0) 
{ 
count++; 
} 
} 
return count;
```

* b) If possible, give a test case that does not execute the fault. If not, briefly explain why not.

x= [1,-2]
* c) If possible, give a test case that executes the fault, but does not result in an error state. 
If not, briefly explain why not. if we have 0 in the test case, it will always execute it

* Program 4

* a) Describe the fault precisely by proposing a modification to the code.
it weong in the logical operator, it must be "&&" while it has "||". Explain what is wrong with the given code. 

```java
public static int oddOrPos(int[] x)
{ 
 int count = 0;
for (int i = 0; i < x.length; i++)
{ 
if (x[i]%2 == 1 && x[i] > 0)
{ 
 count++;
} 
} 
 return count;
```

* b) if possible, give a test case that does not execute the fault. If not, briefly explain why not.
x=[2, -2, 1]
