import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        System.out.print("Type a number of rows: ");
        int rows = scanner.nextInt();
        
        System.out.print("Type a number of columns: ");
        int columns = scanner.nextInt();
        
        int[][] table = new int[rows][columns];
        
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < columns; j++) {
                table[i][j] = i * j;
            }
        }
        System.out.println("Table sheet:");
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < columns; j++) {
                System.out.print(table[i][j] + "\t");
            }   
            System.out.println();
        }
        scanner.close();
    }
    }
