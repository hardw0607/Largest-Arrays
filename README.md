# Largest-Arrays
Largest Arrays
package Arrays;

public class LargestArrays1 {
    public static int getlargest(int numbers[]) {
        int largest = Integer.MIN_VALUE;   // start with very small value
        int smallest = Integer.MAX_VALUE;  // start with very large value

        for (int i = 0; i < numbers.length; i++) {
            if (largest < numbers[i]) {
                largest = numbers[i];   // update largest
            }
            if (smallest > numbers[i]) {
                smallest = numbers[i];  // update smallest
            }
        }

        System.out.println("smallest value " + smallest);
        return largest;  // only largest is returned
    }

    public static void main(String[] args) {
        int numbers[] = { 1, 2, 3, 4, 5 };
        System.out.println("Largest value " + getlargest(numbers));
    }
}
//output 
//smallest value 1
//Largest value 5

