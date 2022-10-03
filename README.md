# Java_solutions

Java task solutions  with Gistr.

- [Integers_divisible_indivisible](https://gist.github.com/MagdalenaOlak/b1b240b7a36ef7faf003e2206d33e4b4) -  Napisz funkcję, która wypisze wszystkie liczby całkowite w zakresie od 1 do stu milionów, które spełniają łacznie następujące warunki:
Są podzielne przez 3 oraz przez 5, a także niepodzielne przez 6.
- [Divisible_indivisible_from_array](https://gist.github.com/MagdalenaOlak/bcdf26dbde0355b300d457ebbc345ac2) -  Napisz funkcję, która wypisze wszystkie liczby z ciągu, które spełniają łacznie następujące warunki:
Są podzielne przez 3 oraz przez 5, a także niepodzielne przez 6.
- [Bubble_Sorting](https://gist.github.com/MagdalenaOlak/cc7c9a8ffbfc8763636f5f0b2e381753) - Sort the array by bubble sorting.
- [Strings_array](https://gist.github.com/MagdalenaOlak/69bbd3dba4a600053fada7f6f5995813) - Ciąg zawieraja liter i cyfry od 0 do 9. Wypisz w konsoli po kolei wszystkie litery a cyfry zacstąp ich słownym odpowiednikiem. 
- [Recursion](https://gist.github.com/MagdalenaOlak/b1fc17a476d11cff012daacc9f09d002) - On the console, write the numbers from 3 to 1, then the word 'Finidhed' and then the numbers from 1 to 3, using recursion.
- [Pyramid3D](https://gist.github.com/MagdalenaOlak/103b41a9287cb8bb4ddea458022dbdbf) - How many blocks are needed to build a 3D pyramid with a height h?
- [Number of words in the string](https://gist.github.com/MagdalenaOlak/baae33b9eb5c4f388c5ad75da18eb521) - How many words are in the given string?
- [Greet the name from array](https://gist.github.com/MagdalenaOlak/fb20c985a242b1bbe8908d9df2f167f5) - Write a program in which you declare and create a five-element array of the appropriate type. In the loop, you will get 5 names from the user and save them in it. Then display "Hello name_ftom_array" notifications on the screen for each of the given parameters.
- [Table_2D_create](https://gist.github.com/MagdalenaOlak/e2b88bdc4d3e6bc3c9d8599d0c03ae98) - Create the multiplication table.
- [Koło - obwód i promień](https://gist.github.com/MagdalenaOlak/ba3a492f9c1ebe60ef40e2b8c06ad406) - Klasa Kolo - pola prywatne (gettery i settery), oraz metody.
- [Kolo1 - Konstruktory](https://gist.github.com/MagdalenaOlak/cc5190cd41ec245774d750dcfa990103) - Klasa Kolo1 z zastosowaniem prostych konstruktorów
- [Kolo2 - Pole statyczne Id oraz konstruktory rekursyjne](https://gist.github.com/MagdalenaOlak/0c84fa014025af56cf6a29573623ca43) - Pole statyczne Id odnoszące się do wszystkich obiektów klasy oraz konstruktory rekursyjne

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
                

- [Count Odd Numbers below n](https://gist.github.com/MagdalenaOlak/80a8d0812af9a435e5eb27d95dc23693) - Given a number n, return the number of positive odd numbers below n. Examples (Input -> Output):
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



- [InvertedTriangleLeft](https://gist.github.com/MagdalenaOlak/92fc65ce108a8fee1dc4b6ece1a74afa) - Draw an inverted equilateral triangle like below with '*' characters taking the number of stars in the base = 6. Each next level should have 1 star less. Enter the number of stars in the triangle.

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





- [Inverted Triangle Right](https://gist.github.com/MagdalenaOlak/b082ae6565ea3e69288643330b6cca53) - Draw an inverted equilateral triangle right like below with '*' characters taking the number of stars in the base = 6. Each next level should have 1 star less. Enter the number of stars in the triangle.

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



     
     
- [Inverted Christmas Tree](https://gist.github.com/MagdalenaOlak/f9b2e822a053362aa35b1123c3300934) - Draw an inverted Christmas tree like below with '*' characters taking the height of 6 levels. Enter the number of stars in the tree.

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


- [Triangle Left](https://gist.github.com/MagdalenaOlak/8eae00c1da6460fd8e083f9ca8da5843)  - Draw an equilateral triangle like below with '*' characters taking the number of stars in the base = 5. Each next level should have 1 star less. Enter the number of stars in the triangle.

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


- []()
