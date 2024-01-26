# DifferenceArraysArrayLists
Difference Arrays Array Lists
import java.util.ArrayList;
import java.util.Arrays;

public class DifferenceArraysArrayLists {

    public static void main(String[] args) {
        // Using Arrays
        int[] intArray = new int[5]; // Creating an array of size 5
        intArray[0] = 1;
        intArray[1] = 2;
        intArray[2] = 3;
        intArray[3] = 4;
        intArray[4] = 5;

        System.out.println("Array Elements: " + Arrays.toString(intArray));

        // Attempting to add a new element to the array (not possible)
        // intArray[5] = 6; // Uncommenting this line would result in an ArrayIndexOutOfBoundsException

        // Using ArrayList
        ArrayList<Integer> intArrayList = new ArrayList<>(); // Creating an ArrayList
        intArrayList.add(1);
        intArrayList.add(2);
        intArrayList.add(3);
        intArrayList.add(4);
        intArrayList.add(5);

        System.out.println("ArrayList Elements: " + intArrayList);

        // Adding a new element to the ArrayList
        intArrayList.add(6);

        System.out.println("Updated ArrayList: " + intArrayList);

        // Demonstrating dynamic resizing of ArrayList
        System.out.println("ArrayList Size: " + intArrayList.size());

        // Accessing elements in both array and ArrayList
        System.out.println("Element at index 2 in Array: " + intArray[2]);
        System.out.println("Element at index 2 in ArrayList: " + intArrayList.get(2));

        // Iterating over array elements
        System.out.print("Array Elements: ");
        for (int i = 0; i < intArray.length; i++) {
            System.out.print(intArray[i] + " ");
        }
        System.out.println();

        // Iterating over ArrayList elements
        System.out.print("ArrayList Elements: ");
        for (int num : intArrayList) {
            System.out.print(num + " ");
        }
    }
}
