using System.ComponentModel.Design;
using System.Threading.Channels;

namespace Mini_Programming_Tasks
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Enter an integer from 0 to 255. This integer will be converted to binary.");
            double userdecimaldouble = Convert.ToDouble(Console.ReadLine());
            if ((userdecimaldouble < 0) || (userdecimaldouble > 255))
            {
                Console.WriteLine("Your integer is not in the range of 0 to 255.");
            }
            else
            {
                int userdecimalint = Convert.ToInt32(userdecimaldouble);

                int division1userint = (userdecimalint / 2);
                int bindig8 = (userdecimalint % 2);

                int division2userint = (division1userint / 2);
                int bindig7 = (division1userint % 2);

                int division3userint = (division2userint / 2);
                int bindig6 = (division2userint % 2);

                int division4userint = (division3userint / 2);
                int bindig5 = (division3userint % 2);

                int division5userint = (division4userint / 2);
                int bindig4 = (division4userint % 2);

                int division6userint = (division5userint / 2);
                int bindig3 = (division5userint % 2);

                int division7userint = (division6userint / 2);
                int bindig2 = (division6userint % 2);

                int division8userint = (division7userint % 2);
                int bindig1 = (division7userint % 2);

                Console.WriteLine("The decimal number " + userdecimalint + " is: " + bindig1 + bindig2 + bindig3 + bindig4 + bindig5 + bindig6 + bindig7 + bindig8 + " in binary.");
            }
        }
    }
}
