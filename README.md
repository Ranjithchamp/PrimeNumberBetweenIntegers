# PrimeNumberBetweenIntegers
public class PrimeNumberBetweenIntegers {

	public static void main(String[] args) {

		Scanner get = new Scanner(System.in);
		System.out.println("enter range for display prime number ");
		int p = get.nextInt();
		int b = get.nextInt();
		int l = 0;
		System.out.println("the Prime numbers are");
		for (int a = p; a <= b; a++) {
			for (int i = 2; i < a / 2; i++) {
				if (a % i == 0) {
					l = 1;
					break;
				}
			}
			if (l == 0) {
				System.out.println(" " + a);
				// count[k++] = a;
			}
			l = 0;
		}
	}

}
