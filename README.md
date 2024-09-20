
import java.util.*;
class Calculator{
    public static void main(String[] args) {
        Scanner obj = new Scanner(System.in);

 
        System.out.println("This is a Simple Calculator.");
        System.out.println("Choose an Option");
        System.out.println("1.Addition");
        System.out.println("2.substraction");
        System.out.println("3.Multipication");
        System.out.println("4.Division");
        System.out.print("Enter your choice (1-4): ");
        int choice = obj.nextInt();
        while (choice < 1 || choice > 4) {
        if (choice < 1 || choice > 4) {
            System.out.println("Invalid choice! Please enter a valid option (1-4).");
            obj.close();
            System.exit(0);
        }
    }


        System.out.println("Enter the value of A:");
        int A = obj.nextInt();
        System.out.println("Enter the value of B:");
        int B = obj.nextInt();
        double result = 0;
        int validChoice = 1;

        switch (choice) {
            case 1:
            result = A+B;
            System.out.println("Result is :" + " " + A + " " + "+" + " " + B + " "  + "=" + " "  + result);
            break;
            case 2:
            result = A-B;
            System.out.println("Result is :" + " "  + A +" " + "-" +  " " + B  + " "  +"=" + " " + result);
            break;
            case 3:
            result = A*B;
            System.out.println("Result is;"+ " "  + A+ " " + "*" + " " + B + " "  + "=" + " "  + result) ;
            break;
            case 4:
            result = A/B;
            System.out.println("Result is :" + " "  + A +" " +"/"+ " "  + B + " "  + "=" + " "  + result);
            default:
                break;
        }
    }
}
