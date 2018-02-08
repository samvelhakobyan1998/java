import java.math.BigInteger;
import java.util.Scanner;

public class SuperLongSums {

	public static void main(String[] args) {
		Scanner input = new Scanner(System.in);
		int digits = input.nextInt();
		String num1 = "", num2 = "";

		for (int digit = 0; digit < digits; digit++) {
			num1 += input.next();
			num2 += input.next();
		}
		num1 = (new BigInteger(num1)).add(new BigInteger(num2)).toString();
		System.out.println(num1);
		
	}
}
