import java.util.Scanner;

public class Main {
    public static <T extends Comparable<T>> void sort(T[] arr) {
        for (int i = 0; i < arr.length - 1; ++i) {
            for (int j = 0; j < arr.length - i - 1; ++j) {
                if (arr[j].compareTo(arr[j+1]) > 0) {
                    T tmp = arr[j];
                    arr[j] = arr[j+1];
                    arr[j+1] = tmp;
                }
            }
        }
    }
    
    public static <T> void print(T[] arr) {
        for (int i = 0; i < arr.length; ++i) {
            System.out.print(arr[i] + (i+1 == arr.length ? "\n" : " "));
        }
    }
    
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        Integer[] arr1 = new Integer[n];
        for (int i = 0; i < n; ++i) arr1[i] = sc.nextInt();
        
        n = sc.nextInt();
        Double[] arr2 = new Double[n];
        for (int i = 0; i < n; ++i) arr2[i] = sc.nextDouble();
        
        n = sc.nextInt();
        String[] arr3 = new String[n];
        for (int i = 0; i < n; ++i) arr3[i] = sc.next();
        
        sort(arr1);
        sort(arr2);
        sort(arr3);
        print(arr1);
        for (int i = 0; i < arr2.length; ++i) System.out.print(arr2[i] + " ");
        System.out.print("\n");
        print(arr3);
    }
}
