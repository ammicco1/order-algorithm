HERE'S THE MAIN SORT ALGORITHM WHICH ARE:
 - INSERTIONSORT 
 - MERGESORT
 - HEAPSORT
 - QUICKSORT

ALL OF THEESE ARE IMPLEMENTED IN C. 

NOW LET'S TAKE A LOOK TO THE COMPLEXITY:
 - INSERTIONSORT IN THE WORST CASE HAS A COMPLEXITY OF O(n^2).
 - MERGESORT IN THE WORST CASE HAS A COMPLEXITY OF O(n logn).
 - HEAPSORT IN THE WORST CASE HAS A COMPLEXITY OF O(n logn).
 - QUICKSORT IN THE WORST CASE HAS A COMPLEXITY OF O(n^2).

ARGUMENTS OF THE ALGORITHMS FUNCTION:
 - INSETIONSORT FUNCTION TAKES:
    - THE ARRAY
    - THE LENGTH OF THE ARRAY 
    AS ARGUMENTS.
 - MERGESORT FUNCTION TAKES:
    - THE ARRAY 
    - THE LOWEST INDEX OF THE ARRAY (QUITE ALWAYS 0)
    - THE HIGEST INDEX OF THE ARRAY (LENGTH - 1)
     AS ARGUMENTS.
 - HEAPSORT FUNCTION TAKES:
    - THE ARRAY
    - THE LENGTH OF THE ARRAY 
    AS ARGUMENTS.
 - QUICKSORT FUNCTION TAKES:
    - THE ARRAY 
    - THE LOWEST INDEX OF THE ARRAY (QUITE ALWAYS 0)
    - THE HIGEST INDEX OF THE ARRAY (LENGTH - 1)
     AS ARGUMENTS.

THE "test.c" FILE CONTAINS THE CODE FOR TESTING THE ALGORITHMS, YOU CAN COMPILE IT WITH THE MAKEFILE AND YOU CAN DECIDE WITH THE CONSTANT \_\_LEN\_\_ AND \_\_MAX_NUM\_\_ THE MAX LENGHT OF THE RANDOM ARRAY AND THE MAX OF THE RANDOM NUMBER.
THE TEST PROGRAM CREATE RANDOM ARRAYS AND LET YOU DECIDE WICH ALGORITHM USE TO SORT THEM. AFTER THAT IT CALCULATE THE TIME OF EXECUTION.
PS. THE TIME OF EXECUTION IS WAY TOO SMALL ON SORTING SMALL ARRAYS, SO IT DISPLAYS 0.000000, IF YOU WANT TO TEST THE ALGORITHMS IN TERMS OF SECOND YOU HAVE TO CREATE ARRAYS THAT CONTAINS MORE THAN 1000/10000 ELEMENTS.

IF YOU USE LINUX USE THE MAKEFILE, IF YOU USE WINDOWS:
 - PASTE THEESE COMMANDS IN CMD TO COMPILE:
    - gcc -Wall -ansi -pedantic -c heapsort.c insertionsort.c mergesort.c quicksort.c test.c
    - gcc -Wall -ansi -pedantic -o test.exe heapsort.o insertionsort.o mergesort.o quicksort.o test.o

- AND THIS TO CLEAN:
    - del *.o 
    - del *.exe