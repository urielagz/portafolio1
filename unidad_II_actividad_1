namespace unidad_II_actividad_1
{
    internal class Program
    {
        static void Main(string[] args)

            
        {
            int cantidad_de_persoanas;

            Console.Write("Ingera la cantidad de personas que desea ingresar: ");
            while (!int.TryParse(Console.ReadLine(), out cantidad_de_persoanas) || cantidad_de_persoanas < 1)
            {
                Console.WriteLine("ERROR Ingresa un numero valido mayor o igual a 1");
                Console.Write("intenta nuevamente");

            }

            List<int> edades = new List<int>();
            List<string> nombres = new List<string>();

            for (int i = 0; i < cantidad_de_persoanas; i++)
            {
                Console.WriteLine($"persona numero: {i+1}");
                Console.Write("Nombre: ");
                string nombre = Console.ReadLine();
                nombres.Add( nombre );
                
                int edad;
                Console.Write("edad: ");
                while (!int.TryParse(Console.ReadLine(), out edad) || edad < 0)
                {
                    Console.WriteLine("ERROR Ingresa una edad valida");
                    Console.Write("intenta nuevamente");
                }
                edades.Add(edad);
            
            }
            if (cantidad_de_persoanas == 1)
            {
                Console.WriteLine($"nombre: {nombres[0]}");
                if (edades[0] >= 18)
                    Console.WriteLine("es mayor de Edad.");
                else
                    Console.WriteLine("Es menor de edad");
            }
            else 
            {
                for (int i = 0; i < cantidad_de_persoanas; i++)
                {
                    Console.WriteLine($"{nombres[i]}-{edades[i]} años ");
                }

                List <string> mayores = new List<string>();
                List <string> menores = new List<string>();

                for (int i = 0; i < cantidad_de_persoanas; i++)
                {
                    if (edades[i] >= 18)

                        mayores.Add($"{nombres[i]}-{edades[i]} años");




                    else
                        menores.Add($"{nombres[i]}-{edades[i]}años");
                      
                }

                if (mayores.Count > 0)
                {
                    Console.WriteLine("Mayores de edad");
                    foreach (string persona in mayores)
                        Console.WriteLine(persona);
                }
                if (menores.Count > 0)
                {
                    Console.WriteLine("Menores de edad");
                    foreach (string persona in menores)
                        Console.WriteLine(persona);
                }
            
            }
            Console.WriteLine("Programa finalizado");

        }
    }
}
