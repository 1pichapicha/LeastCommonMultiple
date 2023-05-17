# LeastCommonMultiple
LeastCommonMultiple
import java.util.Scanner;

public class LeastCommonMultiple {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Введите первое число: ");
        int number1 = scanner.nextInt();

        System.out.print("Введите второе число: ");
        int number2 = scanner.nextInt();

        int lcm = calculateLCM(number1, number2);
        System.out.println("Наименьшее общее кратное: " + lcm);
    }

    public static int calculateLCM(int number1, int number2) {
        int max = Math.max(number1, number2);
        int lcm = max;
        while (true) {
            if (lcm % number1 == 0 && lcm % number2 == 0) {
                return lcm;
            }
            lcm += max;
        }
    }
}
