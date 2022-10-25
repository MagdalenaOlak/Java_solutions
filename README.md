# Java_solutions

Java task solutions  with Gistr.
- [1. Integers_divisible_indivisible](#integers)
- [2. Divisible_indivisible_from_array](#Divisible_indivisible_from_array)
- [3. Bubble_Sorting](#Bubble_Sorting)
- [Strings_array](#Strings_array)
- [Recursion](#Recursion)
- [Pyramid3D](#Pyramid3D)
- [Number of words in the string](#Number-of-words-in-th-string)
- [Greet the name from array](#Greet-the-name-from-array)
- [Table_2D_create](#Table_2D_create)
- [Koło - obwód i promień](#Kolo-obwod--promien)
- [](#)
- [](#)
- [](#)
- [](#)
- [](#)
- [](#)
- [](#)
- [](#)

<a name=""></a>


- <a name="integers"></a>[Integers_divisible_indivisible](https://gist.github.com/MagdalenaOlak/b1b240b7a36ef7faf003e2206d33e4b4) -  Napisz funkcję, która wypisze wszystkie liczby całkowite w zakresie od 1 do stu milionów, które spełniają łacznie następujące warunki:
Są podzielne przez 3 oraz przez 5, a także niepodzielne przez 6.

		public class Integers {

			public static void main(String[] args) {
				// TODO Auto-generated method stub

				for (int i = 1; i <= 100; i++)
			{
			    if (( i % 3 == 0 && i % 5 == 0) && (i % 6 != 0)) // podzielne przez 3 i 5 a niepodzielne przez 6
				System.out.println(i);
			}
		    }
		}


- <a name="Divisible_indivisible_from_array">[Divisible_indivisible_from_array](https://gist.github.com/MagdalenaOlak/bcdf26dbde0355b300d457ebbc345ac2) -  Napisz funkcję, która wypisze wszystkie liczby z ciągu, które spełniają łacznie następujące warunki:
Są podzielne przez 3 oraz przez 5, a także niepodzielne przez 6.

		public class Divisible_nondivisible_from_array {

			public static void main(String[] args) {
				// TODO Auto-generated method stub
				int[] tablica = {1, 15, 48, 45, 88, 75, 85 };

			for (int i = 0; i < tablica.length; i++)
			{
			    if ((tablica[i] % 3 == 0 && tablica[i] % 5 == 0) && (tablica[i] % 6 != 0)) // podzielne przez 3 i 5 a niepodzielne przez 6
			    {
				System.out.println(tablica[i]);
			    }
			}
		    }
		}

 
 
 
- <a name="Bubble_Sorting"></a>[Bubble_Sorting](https://gist.github.com/MagdalenaOlak/cc7c9a8ffbfc8763636f5f0b2e381753) - Sort the array by bubble sorting.

		public class Bubble_Sorting {

			public static void main(String[] args) {
				// TODO Auto-generated method stub

				{ 
					int[] myArray = new int[] { 4, 6, 9, 34, 65, 21, 1, 87, 54 };
					int temp = 0;
					for (int i = 0; i < myArray.length; i++)             
					{                
						for (int j = 0; j < myArray.length - 1; j++)
						{     if (myArray[j] > myArray[j + 1])
							{   temp = myArray[j];                        
								myArray[j] = myArray[j + 1];
								myArray[j + 1] = temp;   
							} 
						} 
					}

					for (int i = 0; i < myArray.length; i++)  
					{                
						System.out.println(myArray[i]); 
					}
				}
			}
		}


- <a name="Strings_array"></a>[Strings_array](https://gist.github.com/MagdalenaOlak/69bbd3dba4a600053fada7f6f5995813) - Ciąg zawieraja liter i cyfry od 0 do 9. Wypisz w konsoli po kolei wszystkie litery a cyfry zacstąp ich słownym odpowiednikiem. 

		public class Strings_array {

			public static void main(String[] args) {
				// TODO Auto-generated method stub
				String[] phrase = {"a", "1", "2", "b", "9", "c", "0" };            

				   String outPut = "";
				   for (String c: phrase)
				   { 
					   if (c == "0")		   	
					   {
						   outPut += "zero";}
					   else if (c == "1")
					   {
						   outPut += "jeden";}
					   else if (c == "2")
					   {
						   outPut += "dwa";}
					   else if (c == "3")
					   {
						   outPut += "trzy";}
					   else if (c == "4")
					   {
						   outPut += "cztery";}
					   else if (c == "5")
					   {
						   outPut += "pięć";}
					   else if (c == "6")
					   {
						   outPut += "sześć";}
					   else if (c == "7")
					   {
						   outPut += "siedem";}
					   else if (c == "8")
					   {
						   outPut += "osiem";}
					   else if (c == "9")
					   {
						   outPut += "dziewięć";}			   
					   else
					   {
						   outPut += c ; 
					   }
					}    

				   System.out.println(outPut);


			}

		}


- <a name="Recursion"></a>[Recursion](https://gist.github.com/MagdalenaOlak/b1fc17a476d11cff012daacc9f09d002) - On the console, write the numbers from 3 to 1, then the word 'Finidhed' and then the numbers from 1 to 3, using recursion.

		public class Recursion {

			public static void main(String[] args) {
				// TODO Auto-generated method stub
				Recursion1 wynik = new Recursion1();
			int a = 3;
			wynik.Rec(a);
			}
		}
		class Recursion1
		{
		    public void Rec(int a)
		    {

			if (a > 0)

			{
				System.out.println(a);
			    Rec(a - 1);
			    System.out.println(a);
			}
			else
				System.out.println("Finished.");
		    }
		}

- <a name="Pyramid3D"></a>[Pyramid3D](https://gist.github.com/MagdalenaOlak/103b41a9287cb8bb4ddea458022dbdbf) - How many blocks are needed to build a 3D pyramid with a height h?

		import java.util.Scanner;

		public class Pyramid3D {

			public static void main(String[] args) {
				// TODO Auto-generated method stub
				 int count = 2;

			 Scanner odczyt = new Scanner(System.in);
			 System.out.println("Podaj wysokość piramidy: ");
				 int h = odczyt.nextInt();
				 odczyt.close();
			 System.out.println("*");
			 for (int i = 1; i <= h-1; i++)
			 {
			     for (int g = 1; g <= (i + 1) * (i + 1); g++)
			     {
				 System.out.print(count);
				 System.out.print("*");                    
				 count++;                    
			     }
			     System.out.println();
			 }
			 System.out.println("Liczba '*': " + (count-1));
			 System.out.println();

			}

		}


- <a name="Number-of-words-in-th-string"></a>[Number of words in the string](https://gist.github.com/MagdalenaOlak/baae33b9eb5c4f388c5ad75da18eb521) - How many words are in the given string?

		import java.util.Scanner;

		public class Ilosc_wyr_w_stringu {

			public static void main(String[] args) {
				// TODO Auto-generated method stub

				Scanner odczyt = new Scanner(System.in);
				System.out.print("Wpisz dowolne zdanie: ");
				String tekst = odczyt.nextLine();
				odczyt.close();
				char[] lit = tekst.toCharArray();
			int liczbaWyrazow = 1;
			for(char litera: lit)
			    if (litera == ' ') liczbaWyrazow++;
			System.out.print("Wprowadzony tekst zawiera wyrazów: " + liczbaWyrazow);        
			}
		}

- <a name="Greet-the-name-from-array"></a>[Greet the name from array](https://gist.github.com/MagdalenaOlak/fb20c985a242b1bbe8908d9df2f167f5) - Write a program in which you declare and create a five-element array of the appropriate type. In the loop, you will get 5 names from the user and save them in it. Then display "Hello name_ftom_array" notifications on the screen for each of the given parameters.

		public class Imiona {

			public static void main(String[] args)  {
				// TODO Auto-generated method stub				

				String[] names = {"Marek", "Anna", "Wojtek", "Sylwia", "Patryk"}; // numeruje się od 0 czyli 0123

				for(String name :names) {
				    System.out.println("Witaj "+ name);	            
			       }				
			}
		}



- <a name="Table_2D_create"></a>[Table_2D_create](https://gist.github.com/MagdalenaOlak/e2b88bdc4d3e6bc3c9d8599d0c03ae98) - Create the multiplication table.

		public class Table_2D_create {

			public static void main(String[] args) {
				// TODO Auto-generated method stub

				int[][] tablica2D = new int[11][11];

				for (int i = 1; i < 11; i++) {

					for (int j = 1; j < 11; j++) {

						tablica2D[i][j]= i*j;
					}
				}

				for (int[] tablica1D : tablica2D) {
				    // dopiero pętla wewnętrzna pobiera liczby
				    for (int liczba : tablica1D) {
					// dla liczb < 10 dodajemy 0 przed cyfrą
					if (liczba < 10) 
					    System.out.print("0"+liczba + ",");
					else
					    System.out.print(liczba + ",");
				    }
				    // nowa linia dla każdej 10-tki liczb
				    System.out.println("");
				}
			}
		}


- <a name="Kolo-obwod--promien"></a>[Koło - obwód i promień](https://gist.github.com/MagdalenaOlak/ba3a492f9c1ebe60ef40e2b8c06ad406) - Klasa Kolo - pola prywatne (gettery i settery), oraz metody.

                    public class Kolo 
                    {
                      private double promien;		
                      public void setPromien(double r) 
                      {
                        this.promien = r;
                      }	
                      public double GetPromien() {
                        return promien;		
                      }
                      public double obliczObwodKola()
                      {
                        double obwod = 2*Math.PI*promien;		
                        return obwod;			
                      }
                      public double obliczPoleKola() {
                        double pole = Math.PI*promien*promien;
                        return pole;		
                      }
                      public static void main(String[] args) 
                      {
                        // TODO Auto-generated method stub

                        Kolo koleczko = new Kolo(); 		
                        koleczko.setPromien(1.0);	
                        System.out.println("Promien kola wynosi: " + koleczko.GetPromien());	
                        System.out.println("Obwod kola wynosi: " + koleczko.obliczObwodKola());
                        System.out.println("Pola kola wynosi: " + koleczko.obliczPoleKola());		
                      }
                    }


- <a name=""></a>[Kolo1 - Konstruktory](https://gist.github.com/MagdalenaOlak/cc5190cd41ec245774d750dcfa990103) - Klasa Kolo1 z zastosowaniem prostych konstruktorów

                    public class Kolo1 
                    {	
                      public Kolo1 ()
                      {
                        promien = 1.0;
                      }	
                      public Kolo1 (double r)
                      {
                        promien = r;
                      }	
                      public Kolo1 (double r, String j)
                      {
                        promien = r;
                        if(j.equals("km"))
                        {
                          promien = promien * 1000;
                        }
                      }	
                      private double promien;	
                      public void setPromien(double r) 
                      {
                        this.promien = r;
                      }	
                      public double GetPromien() {
                        return promien;		
                      }	
                      public double obliczObwodKola()
                      {
                        double obwod = 2*Math.PI*promien;		
                        return obwod;			
                      }
                      public double obliczPoleKola() {
                        double pole = Math.PI*promien*promien;
                        return pole;		
                      }

                      public static void main(String[] args) 
                      {
                        // TODO Auto-generated method stub

                        Kolo1 koleczko = new Kolo1(3.5);

                      System.out.println("Promien kola wynosi: " + koleczko.GetPromien());		
                      System.out.println("Obwod kola wynosi: " + koleczko.obliczObwodKola());
                      System.out.println("Pola kola wynosi: " + koleczko.obliczPoleKola() + "\n");			
                      Kolo1 kolko = new Kolo1(3, "km"); 

                      System.out.println("Promien kola wynosi: " + kolko.GetPromien() + " m");		
                      System.out.println("Obwod kola wynosi: " + kolko.obliczObwodKola() + " m");
                      System.out.println("Pola kola wynosi: " + kolko.obliczPoleKola() + " m"); 
                    }
                  }


- <a name=""></a>[Kolo2 - Pole statyczne Id oraz konstruktory rekursyjne](https://gist.github.com/MagdalenaOlak/0c84fa014025af56cf6a29573623ca43) - Pole statyczne Id odnoszące się do wszystkich obiektów klasy oraz konstruktory rekursyjne

                public class Kolo2 
                {
                        private int id; 
                        private static int nextId; 
                        public int getId()
                        {
                                return id;
                        }	                        
                        public Kolo2 ()
                        {
                                this(1.0); 
                        }                        
                        public Kolo2 (double r)
                        {
                                this(r, "cos");                                                 
                        }                        
                        public Kolo2 (double r, String j)
                        {
                                id=nextId;
                                nextId++; 
                                promien = r;
                                if(j.equals("km"))
                                {
                                        promien = promien * 1000;
                                }
                        }
                        private static Kolo2 koleczko;
                        private double promien;
                        public void setPromien(double r) 
                        {
                                this.promien = r;
                        }	
                        public double GetPromien() {
                                return promien;		
                        }                        
                        public double obliczObwodKola()
                        {
                                double obwod = 2*Math.PI*promien;		
                                return obwod;			
                        }
                        public double obliczPoleKola() {
                                double pole = Math.PI*promien*promien;
                                return pole;		
                        }
                        public static void main(String[] args) 
                        {
                                // TODO Auto-generated method stub		

                                Kolo2[] kolka = new Kolo2[3];
                                kolka[0] = new Kolo2();
                                kolka[1] = new Kolo2(3.5);
                                kolka[2] = new Kolo2(6.5,"km");

                                for (Kolo2 x:kolka)
                                {
                                System.out.println("ID kola wynosi: " + x.getId());
                                System.out.println("Promien kola wynosi: " + x.GetPromien());		
                                System.out.println("Obwod kola wynosi: " + x.obliczObwodKola());
                                System.out.println("Pola kola wynosi: " + x.obliczPoleKola()); 
                                System.out.println();
                                }
                        }
                        static
                        {
                                nextId=1;

                        }

                }
                

- <a name=""></a>[Count Odd Numbers below n](https://gist.github.com/MagdalenaOlak/80a8d0812af9a435e5eb27d95dc23693) - Given a number n, return the number of positive odd numbers below n. Examples (Input -> Output):
        7  -> 3 (because odd numbers below 7 are [1, 3, 5])
        15 -> 7 (because odd numbers below 15 are [1, 3, 5, 7, 9, 11, 13])
        
                import java.util.Scanner;

                public class Kata {

                        public static int oddCount(int n)
                          {    
                            int count = 0;
                            for(int i=0;i<n;i++)
                            {
                              if(i % 2 != 0)
                              {
                                count++;
                              }
                            }
                            return count;
                          }		
                        public static void main(String[] args) {
                                // TODO Auto-generated method stub
                                System.out.println("Podaj liczbę: ");
                            Scanner odczyt = new Scanner(System.in);
                            int n = odczyt.nextInt();
                            odczyt.close();

                            System.out.println("Wynik: " + oddCount(n));
                        }
                }



- <a name=""></a>[InvertedTriangleLeft](https://gist.github.com/MagdalenaOlak/92fc65ce108a8fee1dc4b6ece1a74afa) - Draw an inverted equilateral triangle like below with '*' characters taking the number of stars in the base = 6. Each next level should have 1 star less. Enter the number of stars in the triangle.

<p align="center">
  <img src="https://user-images.githubusercontent.com/66574001/193445531-dcf87bda-39c7-4efd-ae32-00d1ca072f04.png" />
</p>
               

           public class InvertedTriangleLeft 
                {
                        public static void main(String[] args) 
                        {
                                // TODO Auto-generated method stub
                                int count = 1;        
                        int h = 6;
                        for(int i = h; i >=1; i--)
                        {
                            for(int y = i ; y > 0; y--)
                            {
                                System.out.print("*  ");
                                count++;
                            }
                            System.out.println();
                        }
                        System.out.println("Liczba '*': " + count);
                        }
                }





- <a name=""></a>[Inverted Triangle Right](https://gist.github.com/MagdalenaOlak/b082ae6565ea3e69288643330b6cca53) - Draw an inverted equilateral triangle right like below with '*' characters taking the number of stars in the base = 6. Each next level should have 1 star less. Enter the number of stars in the triangle.

<p align="center">
  <img src="https://user-images.githubusercontent.com/66574001/193445459-b94e56ca-f14b-4eb0-bd10-0b0317c40ffe.png" />
</p>

                public class InvertedTriangleRight {

                        public static void main(String[] args) {
                                // TODO Auto-generated method stub
                                int count = 1;                        
                        int h = 6;
                        for(int i = h; i >=1; i--)
                        {
                            for(int x = h - i ; x > 0; x--)
                            {
                                System.out.print("   ");
                            }
                            for(int y = i ; y > 0; y--)
                            {
                                System.out.print("*  ");
                                count++;
                            }
                            System.out.println();
                        }
                        System.out.println("Liczba '*': " + count);
                        }
                }

- <a name=""></a>[Christmas Tree](https://gist.github.com/MagdalenaOlak/bc25d4b66d8b3124e70b45dbdb0bdac3) - Draw a Christmas tree as below with the '*' characters taken from the keyboard. Enter the number of stars in the tree.

<p align="center">
  <img src="https://user-images.githubusercontent.com/66574001/197379153-9bf6f31b-0df4-434b-9042-794036150f1a.jpg" />
</p>

		import java.util.Scanner;

		public class ChrustmasTree {
			public static void main(String[] args)
		    {
			Scanner scanner = new Scanner(System.in);
			Integer hightTree = scanner.nextInt();
			int h = hightTree;
			int count = 1;
			for(int i = 1; i <= h; i++)
			{
			    for(int x = h - i ; x > 0; x--)
			    {
				System.out.print("  ");
			    }
			    for(int y = 2 * i - 1 ; y > 0; y--)
			    {
				System.out.print(" *");
				count++;
			    }
			    System.out.println();
			}
			System.out.println("C '*': " + count);
		    }

		}



     
     
- <a name=""></a>[Inverted Christmas Tree](https://gist.github.com/MagdalenaOlak/f9b2e822a053362aa35b1123c3300934) - Draw an inverted Christmas tree like below with '*' characters taking the height of 6 levels. Enter the number of stars in the tree.

<p align="center">
  <img src="https://user-images.githubusercontent.com/66574001/193446079-b6149092-d3aa-405e-a21e-9f7eccd475db.png" />
</p>



                public class InvertedChristmasTree {
                        public static void main(String[] args) {
                                // TODO Auto-generated method stub
                                int count = 1;        
                        int h = 6;
                        for(int i = h; i >=1; i--)
                        {
                            for(int x = h - i ; x > 0; x--)
                            {
                                System.out.print("  ");
                            }
                            for(int y = 2 * i - 1 ; y > 0; y--)
                            {
                                System.out.print(" *");
                                count++;
                            }
                            System.out.println();
                        }
                        System.out.println("Liczba '*': " + count);
                        }
                }


- <a name=""></a>[Triangle Left](https://gist.github.com/MagdalenaOlak/8eae00c1da6460fd8e083f9ca8da5843)  - Draw an equilateral triangle like below with '*' characters taking the number of stars in the base = 5. Each next level should have 1 star less. Enter the number of stars in the triangle.

<p align="center">
  <img src="https://user-images.githubusercontent.com/66574001/193447293-128c9bd7-b228-4c74-a5b9-e709e86bf33b.png" />
</p>


                public class TriangleLeft {

                        public static void main(String[] args) {
                                // TODO Auto-generated method stub
                                int h = 5;
                        int count = 0;
                        for(int i = 0; i < h; i++)
                        {
                            for(int x = h-i; x <= h; x++)
                            {
                                System.out.print(" *");
                                count++;
                            }
                            System.out.println();
                        }
                        System.out.println("count of stars: "+ count);
                        }
                }

- <a name=""></a>[Triangle Right](https://gist.github.com/MagdalenaOlak/4e147401e44ac0168e18f9255a8aea5e)  - Draw an equilateral triangle like below with '*' characters taken from the keyboard. Each next level should have 1 star more. Enter the number of stars in the triangle.

<p align="center">
  <img src="https://user-images.githubusercontent.com/66574001/197380037-163332c0-c992-40f4-a8b2-a1ea433d7287.jpg" />
</p>


		import java.util.Scanner;

		public class TriangleRight {

			public static void main(String[] args) {


			Scanner scanner = new Scanner(System.in);
			Integer hightTree = scanner.nextInt();
			int h = hightTree;
			int count = 0;
			for(int i = 1; i <= h; i++)
			{
				for(int x = h - i ; x > 0; x--)
				    {
					System.out.print("  ");
				    }        	

				for(int y = h - i; y < h; y++)
			    {
				System.out.print(" *");
				count++;
			    }
			    System.out.println();
			}
			System.out.println("count of stars: "+ count);

			}

		}




- <a name=""></a>[Średnia](https://gist.github.com/MagdalenaOlak/1eb6bfe7fafb333753380c7279828ed1) - A method for calculating the average of any string of digits.


		public class Srednia {

			public static void średnia(int... var)
			{
				double s = 0;
				for(int x: var)
				{
					s = s +x;
				}
				s = s/var.length;
				System.out.println("Średnia wynosi " + s);
			}


			public static void main(String[] args) {
				// TODO Auto-generated method stub

				średnia(1,2,3,4,5);
			}
		}


- <a name=""></a>[ENUM kierunek Swiata i rozmiar pizzy](https://gist.github.com/MagdalenaOlak/de3e1d11f6d6f204c7e580261dd77c49)

- <a name=""></a>[]()

