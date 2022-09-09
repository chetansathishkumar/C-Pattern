# Pattern

## Aim:

## Equipment Required:

## Algorithm:

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
