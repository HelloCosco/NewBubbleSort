# NewBubbleSort
//MyBubbleSort Class
public class BubbleSort {
  
    // Need to sort the elements
    public static void bubble_srt(int array[]) {
      //int varaiables
      //array.length
      //for loop( int variables
      //swap Numbers around
        int n = array.length;
        int k;
        for (int m = n; m >= 0; m--) {
        for (int i = 0; i < n - 1; i++) {
        k = i + 1;
        //if loop and set array with common variables to set Sort
        if (array[i] > array[k]) {
        swapNumbers(i, k, array);
                }
            }
        //printNumber of array
            printNumbers(array);
        }
    }
    //private static void
    //swapNumbers
    //int variables
    //int array
    private static void swapNumbers(int i, int j, int[] array) {
        //int temp with i
        int temp;
        temp = array[i];
        //set array equal to i and j
        array[i] = array[j];
        //int temp with j
        array[j] = temp;
    }
    // private void printNumber
    //int the input with printNumber
    private static void printNumbers(int[] input) {
        //create for loop to get a particular condition is satisfied  
        for (int i = 0; i < input.length; i++) {
          //print input
            System.out.print(input[i] + ", ");
        }
        //Print new line
        System.out.println("\n");
    }
    //int input
    //bubblesort
    //main String
    public static void main(String[] args) {
        int[] input = { 7,4,2,1,3,5,8,6,9,0 };
        bubble_srt(input);
  
    }
}
