# Operators And Loops

## Comparison and logical operators

* Comparison Operators
    * ```==``` Compares two values to see if they are the same.
    * ```!=``` compares two values to see if they are NOT the same.
    * ```===``` compares two vales to check if both data type and value are the same.
    * ```!==``` compares two vales to check if both data type and value are NOT the same.
    * ```>``` checks if the number on the left is greater than the number on the right.
    * ```<``` checks if the number on the right is greater than the number on the left.
    * ```>=``` checks if the number on the left is greater than or equal to the number on the right.
    * ```<``` checks if the number on the right is greater than or equal to the number on the left.
    ----------------

* Logical Operator
    * ```&&``` 
        * ```T && T``` returns ```T```
        * ```T && F``` returns ```F```
        * ```F && T``` returns ```F```
        * ```F && F``` returns ```F```

    * ```||```
        * ```T || T``` returns ```T```
        * ```T || F``` returns ```T```
        * ```F || T``` returns ```T```
        * ```F || F``` returns ```F```

    * ```!```
        * ```!```True returns Fales
        * ```!```Fales returns True
-------------

## Loops

loops check the coditions, if condition return true it will run the code block, and check it again till it returns false.

* Types of loops
    * ```for``` it runs the code specific number of times.

    example
    ``` 
    for(var i = 0; i<10; i++ ) {
        document.write(i);
    }
    ```
    * ```while``` runs the code NOT specific times, the code will continue loop again and again as long as the condition is ```true```.

    [Back to Home](README.md)