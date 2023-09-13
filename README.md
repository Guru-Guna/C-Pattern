# Pattern

## Aim:
To write a C# program for a pascal's triangle.

## Equipment Required:
Visual Studio

## Algorithm:
Step 1:
Create a class.

Step 2:
Use nested for loop.

Step 3:
End the for loop.

## Program:

Developed By: S.THIRISHA
Reg no: 212222230160
```
using System;
namespace condition
{
    public class pascal
    {
        public static void Main(string[] args)
        {
            int rows , Val = 1;
            Console.Write("Enter number of rows: ");
            rows = Convert.ToInt32(Console.ReadLine()); 
            for (int i = 0; i < rows; i++)
            {
                for (int blank = 1; blank < rows - i; blank++)
                {
                    Console.Write(" ");
                }
                for (int j = 0; j <= i; j++)
                {
                    if (i == 0 || j == 0)
                    {
                        Val = 1;
                    }
                    else
                    {
                        Val = Val * (i - j + 1) / j;
                    }
                    Console.Write(Val + " ");
                }
                Console.WriteLine();
            }
        }
    }
}
```

## Output:
![262405335-bcc34e6b-0d61-4b4e-bb2a-ea38a24562e1](https://github.com/Thirisha-s/C-Pattern/assets/120380280/883c5ce1-1f22-4d36-9d1f-47cb41e640d6)

## Result:
Thus the C# program to print the pascal's triangle is executed successfully.
