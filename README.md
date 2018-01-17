# Coin-change-problem
An algorithm that gives the minimum possible ways to make the change of a given amount
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
 
namespace ConsoleApplication34
{
   class Program
   {
       static void Main(string[] args)
       {
 
           int a = 0, c = 0, e = 0,g = 0;
           Console.WriteLine("Enter your amount: ");
          int n = int.Parse(Console.ReadLine());
          if (n > 10)
          {
              a = n / 10;
              n = n %10;
          }
          if (n >= 5)
          {
              c = n /5;
              n =n% 5;
          }
          if (n >= 2)
          {
              e = n/ 2;
              n= n% 2;
          }
          if (n >= 1)
          {
              g = n / 1;
              n = n % 1;
          }
          Console.WriteLine("The coin of 10 is {0} ",a);
          Console.WriteLine("The coin of 5 is {0} ", c);
          Console.WriteLine("The coin of 2 is {0} ", e);
          Console.WriteLine("The coin of 1 is {0} ", g);
          
          Console.ReadLine();
       }
   }
}
 
 
