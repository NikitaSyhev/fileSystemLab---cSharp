using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.IO;

namespace ConsoleApp1   //fileSystemLab
{
    internal class Program
    {
        static void Main(string[] args)
        {
            string path;
            if (args.Length > 0)
            {
                path = args[0];
            }
            else
            {
                path = Environment.CurrentDirectory;
             
            }
            DirectoryInfo myDirInfo = new DirectoryInfo(path);
            foreach (var item in myDirInfo.EnumerateDirectories())
            {
                Console.WriteLine($"Каталог {item}");
            }
            {
                foreach (var item in myDirInfo.EnumerateFiles())
                {
                    Console.WriteLine($"Файл {item} имеет размер {item.Length} байт был изменен {item.LastWriteTime}");
                }
            }
            Console.ReadKey();
            }
        }
    }

