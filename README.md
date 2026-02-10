using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace szamonkeres
{
    internal class Program
    {
        

        public static string Reverse(string s)
        {
            char[] charArray = s.ToCharArray();
            Array.Reverse(charArray);
            return new string(charArray);
        }

        static void Main(string[] args)
        {
            int osszeg = 0;

            for (int i = 0; i < 1000000; i++)
            {
                string szam = i.ToString();

                if (szam == Reverse(szam))
                {
                    string joszambin = Convert.ToString(i, 2);

                    if (joszambin == Reverse(joszambin))
                    {
                        osszeg += i;
                    }
                }
            }

            Console.WriteLine(osszeg);
        }
    }
}

Matrix

public CheckBox[,] matrix = new CheckBox[8, 8]; //[sor, oszlop] 


 for (int y = 0; y < 8; y++)
 {
     for (int x = 0; x < 8; x++)
     {
         matrix[y, x] = new CheckBox();
         matrix[y, x].Location = new Point(57 + y * 20, 120 + x * 20);
         matrix[y, x].AutoSize = false;
         matrix[y, x].Size = new Size(20, 20);
         matrix[y, x].Visible = true;
         matrix[y, x].Enabled = true;
         matrix[y, x].Checked = false;
         matrix[y, x].Text = null;
         Controls.Add(matrix[y, x]);
     }
 }
