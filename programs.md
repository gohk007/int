# Interview Programs

> 1.Print Matrix add 2 to every in same row and in another row add the before row total +2
int height = 4;

 int Total=0;
int printno = 0;
for (int i = 1; i <= Width; i++)
{
printno = Total;
for (int j = 1; j <= height; j++)
{

        if (i == 1 && j == 1) printno = 1;
         else printno += 2;

            Console.Write(printno + " " );
        Total += printno;
    }
    Console.WriteLine(Environment.NewLine);

}

Output:
1 3 5 7

18 20 22 24

102 104 106 108

> 2.Print the Number in Reverse order?

int i=1234;

public static void Main(string[] args)
{
Console.Write("Enter the Number: ");  
 int n = int.Parse(Console.ReadLine());  
 int temp = n,r=0,sum=0;
while(n>0){
r=n%10;  
 sum=(sum\*10)+r;  
 n=n/10;
}
Console.Write("ss"+sum);

}

> Revers a string ?
static void Main(string[] args)  
 {  
 string str = "", reverse = "";  
 int Length = 0;  
 Console.WriteLine("Enter a Word");  
 //Getting String(word) from Console  
 str = Console.ReadLine();  
 //Calculate length of string str  
 Length = str.Length - 1;  
 while(Length>=0)  
 {  
 reverse = reverse + str[Length];  
 Length--;  
 }  
 //Displaying the reverse word  
 Console.WriteLine("Reverse word is {0}",reverse);  
 Console.ReadLine();  
 }

3.Pagenation using Linq Query?

int fromRecords= (Pagenumber-1)*100;
int toRecords=pagenumber*100;

List<int> integerList= (from integer in integerList
Select integer).Skip(fromRecords).Take(toRecords).ToList();
