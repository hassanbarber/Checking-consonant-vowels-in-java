# Checking-consonant-vowels-in-java
Checking consonant vowels in java
import java.util.Scanner;
class KiemTraNguyenAm
{
     public static void main(String[ ] arg)
     {
         boolean isVowel=false;;
         Scanner scanner=new Scanner(System.in);
         System.out.println("Enter the character to be checked : ");
         char ch=scanner.next().charAt(0);
         scanner.close();
         switch(ch)
         {
             case 'a' :
             case 'e' :
             case 'i' :
             case 'o' :
             case 'u' :
             case 'A' :
             case 'E' :
             case 'I' :
             case 'O' :
             case 'U' : isVowel = true;
         }
         if(isVowel == true) {
             System.out.println(ch+" Is a vowel");
         }
         else {
             if((ch>='a'&&ch<='z')||(ch>='A'&&ch<='Z'))
                 System.out.println(ch+" Is a consonant");
             else
                 System.out.println("Not in the alphabet!");
         }
     }
}
