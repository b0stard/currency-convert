
import java.util.Scanner;

public class Crawler {
    public static void main(String[] args) {
        int choise;
        double amount;
        double dollar, yuan, euro;

        Scanner sc = new Scanner(System.in);

        System.out.println("Options:");
        System.out.println("Enter 1:Dollar");
        System.out.println("Enter 2:Yuan");
        System.out.println("Enter 3:Euro");

        System.out.println("Choose your is option");
        choise = sc.nextInt();
        System.out.println("you number is:" + choise);

        System.out.println("Enter the amount you want to convert:");
        amount = sc.nextFloat();
        System.out.println("Your amount is:" + amount);



        switch (choise) {
            case 1:
                yuan = amount * 7.24;
                System.out.println(amount + " Dollar = " + yuan + " Yuan ");

                euro = amount * 0.92049;
                System.out.println(amount + " Dollar = " + euro + " Euro ");
                break;
            case 2:
                dollar = amount * 0.138192;
                System.out.println(amount + " Yuan = " + dollar + " Dollar ");

                euro = amount * 0.127205;
                System.out.println(amount + " Yuan = " + euro + " Euro ");
                break;
            case 3:
                dollar = amount * 1.09;
                System.out.println(amount + " Euro = " + dollar + " Dollar ");

                yuan = amount * 7.86;
                System.out.println(amount + " Euro = " + yuan + " Yuan ");
                break;
        }
    }
}
