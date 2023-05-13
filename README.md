# musical-potato
aqui está um exemplo simples de interface em C# usando o .NET Framework:
using System;

namespace MeuPrograma
{
    interface IAnimal
    {
        void EmitirSom();
    }

    class Cachorro : IAnimal
    {
        public void EmitirSom()
        {
            Console.WriteLine("Au au!");
        }
    }

    class Gato : IAnimal
    {
        public void EmitirSom()
        {
            Console.WriteLine("Miau!");
        }
    }

    class Program
    {
        static void Main(string[] args)
        {
            IAnimal animal = new Cachorro();
            animal.EmitirSom();

            animal = new Gato();
            animal.EmitirSom();
        }
    }
}
