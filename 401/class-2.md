# Java loops

**For Loop**
- A loop thats controlled by incrementing a loop counter.

**While Loop**
- Reapeats a statement while it's controlling boolean is true.

**Do While**
- same as a while loop, the first iteration hapens no matter if the while statement is true or false.

# Arrays

**Syntax of declaring a variable**
````
dataType[] arrayRefVar;
or
dataType arrayRefVar[];
````

**To create a new array**
````
arrayRefVar = new dataType[arraySize];
````
- creates an array using new dataType[arraySize].

- assigns the reference of the newly created array to the variable arrayRefVar.

**Combining into one statement**
````
dataType[] arrayRefVar = new dataType[arraySize];
````
**Literal array creation**
````
dataType[] arrayRefVar = {value0, value1, ..., valuek};
````
**For each loop example**

````
public class TestArray {

   public static void main(String[] args) {
      double[] myList = {1.9, 2.9, 3.4, 3.5};

      // Print all the array elements
      for (double element: myList) {
         System.out.println(element);
      }
   }
}
````

### resources
[Different types of loops in Java](https://www.baeldung.com/java-loops)

[Java Arrays](https://www.tutorialspoint.com/java/java_arrays.htm)

