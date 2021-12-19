# java-calculator
Java code for calculator using Exception handling
import java.util.*;
public class Calculator
{
    public static void main(String[] args) {
        int x=1;
        do {
            try {
                System.out.println("Menu");
                System.out.println("1-Addition");
                System.out.println("2-Subtraction");
                System.out.println("3-Multiplication");
                System.out.println("4-Divison");
                System.out.println("5-Modulos");
                System.out.println("6-Exit");
                System.out.println("Choose option: ");
                Scanner scan = new Scanner(System.in);
                int choice = scan.nextInt();  


                switch (choice) {
                    case 1: 
                        System.out.print("Input two numbers:");
                        String dimension = scan.nextLine();
                                String[] parts = dimension.split(" ");
                                int a = Integer.parseInt(parts[0]);
                                int b = Integer.parseInt(parts[1]);
                                int c=a+b;
                                System.out.println("Sum = " +c);
                            break;  
                    case 2: 
                        System.out.print("Input two numbers:");
                        String dif = scan.nextLine();
                                String[] difference = dif.split(" ");
                                int num1 = Integer.parseInt(difference[0]);
                                int num2 = Integer.parseInt(difference[1]);
                                    int d=num1-num2;
                                    System.out.println("Difference = " +d);
                        break;
                    case 3: 
                        System.out.print("Input two numbers:");
                        String multi = scan.nextLine();
                                String[] product = multi.split(" ");
                                int num3 = Integer.parseInt(product[0]);
                                int num4 = Integer.parseInt(product[1]);
                                int p=num3*num4;
                                System.out.println("Product = " +p);
                        break;  
                    case 4: 
                        System.out.print("Input two numbers:");
                        String div = scan.nextLine();
                                String[] quotient = div.split(" ");
                                int num5 = Integer.parseInt(quotient[0]);
                                int num6 = Integer.parseInt(quotient[1]);
                                int q=num5/num6;
                                System.out.println("Quotient = " +q);
                         break;
                    case 5: 
                        System.out.print("Input two numbers:");
                        String mod = scan.nextLine();
                                String[] modulo = mod.split(" ");
                                int num7 = Integer.parseInt(modulo[0]);
                                int num8 = Integer.parseInt(modulo[1]);
                                int m=num7%num8;
                                System.out.println("Modulos = " +m);
                        break;
                    case 6: 
                        System.out.println("Now exiting program...");
                        break;  
                }
            } catch (Exception e) {
               System.out.println("Wrong input. Try again.");
            }
        } while (x==1);
    } 
}
