# Recursive-function

##Aim: To write a C# program to reverse a number using recursive function.

##Algorithm:

##Program:
```
Developed by: Harini.B
Reg. No: 212221230035
```
```
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace exp7
{
    class Program
    {
        public static int m, reverse = 0;
        public static int J(int n)
        {
            if(n>0)
            {
                m = n % 10;
                reverse = reverse * 10 + m;
                n /= 10;
                return J(n);
            }
            return reverse;
        }
        static void Main(string[] args)
        {
            int num;
            Console.WriteLine("Enter a number: ");
            num = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("Reverse of the number: ");
            Console.WriteLine(J(num));
        }
    }
}

```

##Output:
![image](https://github.com/HariniBaskar/Recursive-function/assets/93427253/6f90d25b-aeac-470d-9e2b-028c24e49d96)

##Result:

