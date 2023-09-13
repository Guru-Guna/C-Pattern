# Pattern

## Aim:
To write a C# program for a pascal's triangle.

## Equipment Required:
Visual Studio

## Algorithm:
Step 1:
Start the execution, create a class.

Step 2:
Declare the required integer variables.

Step 3 :
Initialize the value of the variable as 0 for i and j.

Step 4 :
Enter the limits and initialize a for loop for the concept of pascal's triangle.

Step 5 :
Stop the execution..

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
