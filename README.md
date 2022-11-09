# Comp-5.3
Writes a program that determines and prints the number of odd, even, and zero digits in an integer read from the keyboard.
import java.util.Scanner;
public class Comp53 {


    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        int num;
        int odd = 0, even = 0, zero = 0;
        
        System.out.println("Enter a number: ");
        num = scan.nextInt();
        
        while (num != 0){
            int digit = num % 10;
            num = num/10;
            
        if (digit == 0){
            zero++;
        }
        else if(digit % 2 == 0){
            even++;
        }
        else {
            odd++;
        }
    }
        System.out.println("Even Digits: " + even);
        System.out.println("Odd Digits: " + odd);
        System.out.println("Zero Digits: " + zero);
    }
    
}
