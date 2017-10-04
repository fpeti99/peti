# 

// NEGYZETÖSSZEG 


            /*int[] szamok = new int[10];
            int negyzet = 0;
            for(int i = 0; i < 10; i++)
            {
                Console.WriteLine("Add meg az " + (i + 1) + ". számot!");
                szamok[i] = int.Parse(Console.ReadLine());
            }

            for(int i = 0; i < 10; i++)
            {
                negyzet = negyzet + (szamok[i]) * (szamok[i]);
            }
            Console.WriteLine("\nA megadott számok négyzetösszege {0}.", negyzet);
            Console.ReadLine();*/





            //NEGATÍV SZÁMOKAT MEGKERESI -----------------------------------------


            /*int[] tomb = new int[10];
            Random rnd = new Random();
            int db = 0;
            for(int i = 0; i < 10; i++)
            {
                tomb[i] = rnd.Next(-10000,10000);
            }
            for (int i = 0; i < 10; i++)
            {
                Console.WriteLine("A(z) " + (i+1) + ". szám: " + tomb[i]);
            }
            Console.WriteLine();
            for(int i = 0; i < 10; i++)
            {
                if(tomb[i] < 0)
                {
                    Console.WriteLine("A(z) " + (i + 1) + ". szám negatív.");
                    db++;
                }
            }
            Console.WriteLine();
            Console.WriteLine("A negatív elemek száma: " + db);
            Console.ReadLine();*/




            // 10 SZÁM ÁTLAG ÉS SZÓRÁSNÉGYZET -------------------------------------------

            /*int[] szam = new int[10];
            int sum = 0;
            double atlag;
            double szoras = 0;
            for(int i = 0; i < 10; i++)
            {
                Console.WriteLine("Kérdem adja meg a(z) {0}. számot!", (i + 1));
                szam[i] = int.Parse(Console.ReadLine());
                sum = sum + szam[i];
            }
            atlag = sum / 10.0;

            for(int i = 0; i < 10; i++)
            {
                szoras = szoras + (szam[i] - atlag)*(szam[i] - atlag);
            }
            Console.WriteLine("A megadott számok szórásnégyzete {0}, átlaga {1}.", (szoras/10.0), atlag);
            Console.ReadLine();*/




            // FIBONACCI SZÁMOK N-IG -------------------------------------------------------


            /*int n, elso = 0, masodik = 1, kovetkezo = 0;

            Console.WriteLine("Kérem adja meg, hogy meddig írjam ki a Fibonacci számokat!");
            n = int.Parse(Console.ReadLine());

            while((elso+masodik) < n)
            {
                kovetkezo = elso + masodik;
                elso = masodik;
                masodik = kovetkezo;
                Console.Write(kovetkezo + "  ");
            }

            Console.ReadLine(); */

            // SOROZATOK METSZETE ------------------------------------------------------- 

            /*const int an = 15, bn = 10;
            int[] a = new int[an];
            int[] b = new int[bn];

            int[] c = new int[Math.Min(an, bn)];
            Random rand = new Random();

            int i, j, k = 0;

            a[0] = rand.Next(20);
            i = 1;

            bool azonos;


            while(i < an)
            {
                a[i] = rand.Next(20);
                azonos = false;

                for (j = 0; j < i; j++)
                {
                    if (a[i] == a[j])
                    {
                        azonos = true;
                        break;
                    }
                }

                if (azonos == false)
                {
                    i++;
                }
            }

            b[0] = rand.Next(20);
            i = 1;

            while (i < bn)
            {
                b[i] = rand.Next(20);
                azonos = false;

                for (j = 0; j < i; j++)
                {
                    if (b[i] == b[j])
                    {
                        azonos = true;
                        break;
                    }
                }

                if (azonos == false)
                {
                    i++;
                }
            }

            for(i = 0; i < an; i++)
            {
                Console.Write("a[{0}]:{1}  ", i, a[i]);
            }

            Console.WriteLine("\n");

            for (i = 0; i < bn; i++)
            {
                Console.Write("b[{0}]:{1} ", i, b[i]);
            }

            Console.WriteLine("\n");

            for(i = 0; i < an; i++)
            {
                for(j = 0; j < bn; j++)
                {
                    if(a[i] == b[j])
                    {
                        c[k] = a[i];
                        k++;
                    }
                }
            }

            for (i = 0; i < k; i++)
            {
                Console.Write(" c[{0}]:{1} ", i, c[i]);
            }

            Console.ReadLine();*/


            // MÁTRIIIIX ----------------------------------------------------------------------------

            /*int m, n;
            int[,] matrix;

            Console.WriteLine("Kérem adja meg a mátrix sorainak számát!");
            m = int.Parse(Console.ReadLine());
            Console.WriteLine("Kérdem adja meg a mátrix oszlopainak számát!");
            n = int.Parse(Console.ReadLine());

            matrix = new int[m, n];

            for (int i = 0; i < m; i++)
            {
                for (int e = 0; e < n; e++)
                {
                    Console.WriteLine("Adja meg a(z) {0}. sor, {1}. oszlop elemét!", i, e);
                    matrix[i, e] = int.Parse(Console.ReadLine());
                }
            }

            for(int i = 0; i < m; i++)
            {
                for (int e = 0; e < n; e++)
                {
                    Console.Write(matrix[i, e] + " ");
                }
                Console.WriteLine();
            }
            for (int i = 0; i < m; i++)
            {
                for (int e = 0; e < n; e++)
                {
                    if(i == e)
                    {
                        Console.Write(matrix[i, e] + " ");
                    }
                    else
                    {
                        Console.Write("  ");
                    }
                }
                Console.WriteLine();
            }
            Console.ReadKey(); */



            //MÁTRIX --------------------------------------------------------


            /*int n;
            int[,] matrix;
            bool szimmetrikus = true;


            Console.Write("Kérdem adja meg a mátrix dimenzióját: ");
            n = int.Parse(Console.ReadLine());
            matrix = new int[n, n];

            for(int i = 0; i < n; i++)
            {
                for(int j = 0; j < n; j++)
                {
                    Console.WriteLine("Adja meg a mátrix {0}. sorának és {1}. sorának elemét!", i, j);
                    matrix[i, j] = int.Parse(Console.ReadLine());

                }
            }


            for (int i = 0; i < n; i++)
            {
                Console.WriteLine();
                for (int j = 0; j < n; j++)
                {
                    Console.Write(matrix[i, j] + " ");
                }
                
            }

            Console.WriteLine("\n\nA főátló elemei a következők: ");

            for (int i = 0; i < n; i++)
            {
                Console.WriteLine();
                for (int j = 0; j < n; j++)
                {
                    if(i == j)
                    {
                        Console.Write(matrix[i, j] + " ");
                    }
                    else
                    {
                        Console.Write("  ");
                    }

                    if (matrix[i,j] != matrix[j, i])
                    {
                        szimmetrikus = false;
                    }
                }
            }

            Console.WriteLine();

            if(szimmetrikus == true)
            {
                Console.WriteLine("\nA mátrix szimmetrikus.");
            }
            else
            {
                Console.WriteLine("\nA matárix nem szimmetrikus.");
            }





            Console.ReadLine(); */

            // n*n-es mátrix, véletlenül töltse fel 0 és 10 között, jelenitsd meg, kérj be egy számot, szorozd be a mátrixot a számmal  

            int n;
            Console.Write("Kérdem adja meg hány dimenziós legyen a mátrix: ");
            n = int.Parse(Console.ReadLine());

            int[,] matrix = new int[n, n];
            Random rnd = new Random();

            for(int i = 0; i < n; i++)
            {
                for(int j = 0; j < n; j++)
                {
                    matrix[i, j] = rnd.Next(10);
                }
            }

            for (int i = 0; i < n; i++)
            {
                Console.WriteLine();
                for (int j = 0; j < n; j++)
                {
                    Console.Write(matrix[i, j] + " ");
                }
            }


            Console.WriteLine("\nAdja meg a számot, amivel meg szeretné szorozni a mátrixot!");
            int x = int.Parse(Console.ReadLine());


            for (int i = 0; i < n; i++)
            {
                Console.WriteLine();
                for (int j = 0; j < n; j++)
                {
                    Console.Write((matrix[i, j]*x) + "  ");
                }
            }

            Console.ReadLine();
            
            
            
            
            // mátrixot random elemekkel, transzponálja a program, (= a mátrix sorai és oszlopai helyet cserélnek) 

            Console.Write("Adja meg hány dimenziós mátrixot szeretne: ");
            int n = int.Parse(Console.ReadLine());

            int[,] matrix = new int[n, n];
            Random rnd = new Random();

            for(int i = 0; i < n; i++)
            {
                for(int j = 0; j < n; j++)
                {
                    matrix[i, j] = rnd.Next(10,30);
                }
            }

            for (int i = 0; i < n; i++)
            {
                Console.WriteLine();
                for (int j = 0; j < n; j++)
                {
                    Console.Write(matrix[i, j] + "  ");
                }
            }

            Console.WriteLine();

            for (int i = 0; i < n; i++)
            {
                Console.WriteLine();
                for (int j = 0; j < n; j++)
                {
                    Console.Write(matrix[j,i] + "  ");
                }
            }

            Console.ReadLine();
            
            
            
            
            
            
            
            
            // mátrixot random elemekkel, transzponálja a program ugy hogy nem négyzet alakú.

            Console.Write("Adja meg hány soros mátrixot szeretne: ");
            int n = int.Parse(Console.ReadLine());


            Console.Write("Adja meg hány oszlopos mátrixot szeretne: ");
            int m = int.Parse(Console.ReadLine());

            int[,] matrix = new int[n, m];
            int[,] transzp = new int[m, n];

            Random rnd = new Random();

            for(int i = 0; i < n; i++)
            {
                for(int j = 0; j < m; j++)
                {
                    matrix[i, j] = rnd.Next(10,30);
                }
            }

            for (int i = 0; i < n; i++)
            {
                Console.WriteLine();
                for (int j = 0; j < m; j++)
                {
                    Console.Write(matrix[i, j] + "  ");
                    transzp[j, i] = matrix[i, j];
                }
            }

            Console.WriteLine();

            for (int i = 0; i < m; i++)
            {
                Console.WriteLine();
                for (int j = 0; j < n; j++)
                {
                    Console.Write(transzp[i,j] + "  ");
                }
            }

            Console.ReadLine();

