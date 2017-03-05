# Calculadora-B-sica
Calculadora con sus funciones básicas (suma, resta, multiplicación y división)

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Threading;

namespace Calculadora
{
    class Calculadora
    {
        static void Main(string[] args)
        {
            int x1, x2, y;
            string operacion, opcion1;

        inicio:
            Thread.Sleep(1000);
            Console.ForegroundColor = ConsoleColor.Gray;
            Console.WriteLine("Bienvenido a 'Calculadora Basica 0.1' Hecha por: Israel Betanzos");
            Thread.Sleep(1000);
            Console.WriteLine("Que operacion desea llevar acabo?");
            Console.ForegroundColor = ConsoleColor.Yellow;
            Thread.Sleep(1000);
            Console.WriteLine("+ = Suma");
            Console.ForegroundColor = ConsoleColor.Red;
            Thread.Sleep(100);
            Console.WriteLine("- = Resta");
            Console.ForegroundColor = ConsoleColor.Green;
            Thread.Sleep(100);
            Console.WriteLine("* = Multiplicacion");
            Console.ForegroundColor = ConsoleColor.Cyan;
            Thread.Sleep(100);
            Console.WriteLine("/ = Division");
            Console.WriteLine("");
            Console.ForegroundColor = ConsoleColor.White;
            operacion = Console.ReadLine();
            switch (operacion)
            {
                case "+":
                    Console.ForegroundColor = ConsoleColor.Yellow;
                    Console.Clear();
                    Thread.Sleep(800);
                    Console.WriteLine("Haz elegido Modo: Suma");
                    Thread.Sleep(1000);
                    Console.Write("Primer valor a sumar: ");
                    x1 = Convert.ToInt16(Console.ReadLine());
                    Console.Write("Segundo valor a sumar: ");
                    x2 = Convert.ToInt16(Console.ReadLine());
                    Thread.Sleep(800);
                    Console.Write("Resultado = ");
                    y = x1 + x2;
                    Thread.Sleep(400);
                    Console.WriteLine(y);
                    Thread.Sleep(800);
                    goto AfterOptions;

                case "-":
                    Console.ForegroundColor = ConsoleColor.Red;
                    Console.Clear();
                    Thread.Sleep(800);
                    Console.WriteLine("Haz elegido Modo: Resta");
                    Thread.Sleep(1000);
                    Console.Write("Primer valor a restar: ");
                    x1 = Convert.ToInt16(Console.ReadLine());
                    Console.Write("Segundo valor a restar: ");
                    x2 = Convert.ToInt16(Console.ReadLine());
                    Thread.Sleep(800);
                    Console.Write("Resultado = ");
                    y = x1 - x2;
                    Thread.Sleep(400);
                    Console.WriteLine(y);
                    Thread.Sleep(800);
                    goto AfterOptions;

                case "*":
                    Console.ForegroundColor = ConsoleColor.Green;
                    Console.Clear();
                    Thread.Sleep(800);
                    Console.WriteLine("Haz elegido Modo: Multiplicacion");
                    Thread.Sleep(1000);
                    Console.Write("Primer valor a multiplicar: ");
                    x1 = Convert.ToInt16(Console.ReadLine());
                    Console.Write("Segundo valor a multiplicar: ");
                    x2 = Convert.ToInt16(Console.ReadLine());
                    Thread.Sleep(800);
                    Console.Write("Resultado = ");
                    y = x1 * x2;
                    Thread.Sleep(400);
                    Console.WriteLine(y);
                    Thread.Sleep(800);
                    goto AfterOptions;

                case "/":
                    Console.ForegroundColor = ConsoleColor.Red;
                    Console.Clear();
                    Thread.Sleep(800);
                    Console.WriteLine("Haz elegido Modo: Division");
                    Thread.Sleep(1000);
                    Console.Write("Primer valor a dividir: ");
                    x1 = Convert.ToInt16(Console.ReadLine());
                    Console.Write("Segundo valor a dividir: ");
                    x2 = Convert.ToInt16(Console.ReadLine());
                    Thread.Sleep(800);
                    Console.Write("Resultado = ");
                    y = x1 / x2;
                    Thread.Sleep(400);
                    Console.WriteLine(y);
                    Thread.Sleep(800);
                    goto AfterOptions;
            }
            AfterOptions:
            Console.ForegroundColor = ConsoleColor.Gray;
            Console.WriteLine("");
            Console.WriteLine("Deseas continuar?");
            Console.WriteLine("");
            Thread.Sleep(800);
            Console.WriteLine("Menu - Regresar a seleccion de Operacion");
            Console.WriteLine("Salir - Salir del programa");
            Console.WriteLine("");
            opcion1 = Console.ReadLine();
            switch (opcion1)
            {
                case "Menu":
                    Console.Clear();
                    goto inicio;
                case "Salir":
                    Console.WriteLine("");
                    Thread.Sleep(200);
                    Console.WriteLine("Nos vemos la proxima! :)");
                    Thread.Sleep(1000);
                    break;
            }
        }
    }
}

