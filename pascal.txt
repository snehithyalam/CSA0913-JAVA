public class pattern {
  public static void main(String[] args) {
      int n = 5; // Number of rows

      for (int i = 0; i < n; i++) {
          // Print leading spaces
          for (int j = 0; j < n - i - 1; j++) {
              System.out.print("\t");
          }

          int number = 1;
          // Print Pascal's Triangle numbers
          for (int j = 0; j <= i; j++) {
              System.out.print(number + "\t\t");
              number = number * (i - j) / (j + 1);
          }

          System.out.println();
      }
  }
}
