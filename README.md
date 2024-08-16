using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace AplikasListBilanganPrima
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("                Aplikasi List");
            Console.WriteLine("                Bilangan Prima");
			
            Console.WriteLine("========================================================================================================================");
            Console.WriteLine("Nama  : Rizqi fakhrianto");
            Console.WriteLine("Kelas : X PPLG");
            Console.WriteLine("Absen : 30");
            Console.WriteLine("========================================================================================================================");


            for (int num = 2; num <= 1000; num++)//Melakukan looping dari bilangan 2 hingga 1000
            {
                bool isPrima = true;//Menetapkan bilangan prima menjadi isPrimme dan membuat isPrime menjadi true
                for (int pembagi = 2; pembagi <= Math.Sqrt(num); pembagi++)//Melakukan loop dari 2 hingga ke akar kuadrat dari num
                {
                    if (num % pembagi == 0)//Jika num habis dibagi oleh angka di dalam loop 
                    {
                        isPrima = false;//Maka isPrime diatur menjadi false
                        break;//Maka akan di berhentikan
                    }
                }

                
                if (isPrima)//Jika setelah melakukan loop isPrime masih true
                {
                    Console.WriteLine(num + " ");//Maka num yang telah di filter akan ditampilkan ke dalam list bilangan prima pada console
                }
            }
        }
    }
}
  

