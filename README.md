# Pattern
## Aim:
Develop a C# program to print Pascal's Triangle.

## Algorithm:
## STEP 1: 
Create the class and assign the number of rows to be as 5. <br>
## STEP 2:
Run the outer for loop n times. <br>
## STEP 3:
The first inner for loop should print the spaces first. <br>
## STEP 4: 
The second inner for loop should print number using the combination formula. <br>
## STEP 5: 
Display the Results. <br>
## Program:
 ```
 using System;

namespace pattern
{
    class program
    {
        public static void Main()
        {
            int rows = 5, val = 1, blank, i, j;
            for (i = 0; i < rows; i++)
            {
                for (blank = 1; blank <= rows - i; blank++)
                    Console.Write(" ");
                for (j = 0; j <= i; j++)
                {
                    if (j == 0 || i == 0)
                        val = 1;
                    else
                        val = val * (i - j + 1) / j;
                    Console.Write(val + " ");
                }
                Console.WriteLine();
            }
        }
    }

}
```

## Output:
![image](https://user-images.githubusercontent.com/75260837/189271919-8477ea0e-fd42-45b9-8f2e-80e62a064cd6.png)


## Result:
Thus the C# program to print the first 5 rows in a Pascal's traingle has been implemented successfully.
