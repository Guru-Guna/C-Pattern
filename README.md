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

Developed By: Gunaseelan G
Reg no: 212221230031
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
![pattern](https://github.com/Guru-Guna/C-Pattern/assets/93427255/13930931-b97c-44cc-85e7-75e9aa4c634c)

## Result:
Thus the C# program to print the pascal's triangle is executed successfully.
