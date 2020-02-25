# Number-Search-in-the-Array-JAVA
 The program that searches for the number received from the user in the defined Array. Do not forget to import library for the scanner
 
    import java.util.Scanner;

    public class Main {
    public static void main(String[] args) {
        int[] myList = new int[] {2,3,5,7,11,13,17,19,23,29,31,37,41};
        int i;
        boolean isThere = false;
        System.out.print("Enter a number to search in array: ");
        Scanner input = new Scanner(System.in);
        i = input.nextInt();

        for(int number: myList){
            if(number == i){
                isThere = true;
                break;
            }
        }
        if(isThere){
            System.out.println(i + " is available in this array! \n");
            System.out.print("Elements of array: ");
            for(int number: myList) {
                System.out.print(number + " ");
            }
        }else {
            System.out.println(i + " is not available in this array!");
            System.out.print("Elements of array: ");
            for(int number: myList) {
                System.out.print(number + " ");
            }
         }
       }
    }
