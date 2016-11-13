# Ushtrimi2
<pre>
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Text.RegularExpressions;
namespace usht3micro
{
    class Program
    {
        static void Main(string[] args)
        {
            string str = "Microsoft announced its next generation C# compiler today. It uses advanced parser and special optimizer for Microsoft CLR";
            Console.WriteLine(str);
            string[] str3 = str.Split(' ');
            rep(str3);
            Console.ReadLine();
        }
        public static void rep(string[] word)
        {
            string[] strArry1 = new string[] { "C#", "Microsoft", "CLR" };
            string[] strArry2 = new string[] { "**", "*********", "***" };
            for (int j = 0; j < strArry1.Count(); j++)
            {
                for (int i = 0; i < word.Count(); i++)
                {
                    if (word[i] == strArry1[j])
                    {
                        word[i] = strArry2[j];
                    }
                    
                }
            }
            for (int i = 0; i < word.Count(); i++)
            {
                Console.Write(word[i] + " ");

            } 
        }
    }
}
</pre>
