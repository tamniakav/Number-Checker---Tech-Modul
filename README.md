# Number-Checker---Tech-Modul
Just another repository
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _2.Number_Checker
{
    class Program
    {
        static void Main(string[] args)
        {
            string num = Console.ReadLine();
            long number;
            bool isInteger = long.TryParse(num, out number);

            if (!isInteger)
            {
                Console.WriteLine("floating-point");
                return;
            }

            Console.WriteLine("integer");
        }
    }
}
