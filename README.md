# Aula02

> CORRIJIR CODIGO

using System;
using System.Collections.Generic;
using System.Globalization;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace CalculadoraNotas
{
    internal class Program
    {
        static void Main(string[] args)
        {
            //1+1= 11 => Concatenar 
            //1+1 = 2
            //String => Numero
            //Primeira Etapa => Utilizar Variavel
            //Tipo de Variavel => int, decimal, float, double, long
            //Segunda Etapa => Declarar 
            //Terceira Etapa => Atribuir Valor

            //Console.ReadLine() =String
            //Variavel = double => CAST => Convert  


            double nota1, nota2, media; 

         


            Console.WriteLine("Entrada da Nota1:");
            nota1 = converterNota(Console.ReadLine());

            Console.WriteLine("Entrada da Nota2:");
            nota2 = Convert.ToDouble(Console.ReadLine());

            media = CalculoNota(nota1, nota2, media);

            //Console.WriteLine("A média do Aluno é: " + media + nota1 + nota2);
            //Console.WriteLine(String.Format("A média do Aluno é: (0)", media, nota1, nota2));
            Console.WriteLine($"A média do Aluno é: {media}, nota1: {nota1}, nota2 {nota2}");
        }


        // função - metodo 
         private static void montarRotulo(string mensagem)
        {

            Console.WriteLine(mensagem);
            

        }

        private static double converterNota(string nota)
        {


            double notaConvertida;
            notaConvertida = Convert.ToDouble(nota);
            return notaConvertida;

        }

        private static double CalculoNota(double nota1, double nota2, double media)
        {


            media = (nota1 + nota2) / 2;
            return media; 

        }


    }
}


// função - metodo 
// private string MontarRota 


