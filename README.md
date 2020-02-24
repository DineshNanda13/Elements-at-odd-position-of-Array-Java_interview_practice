# Elements-at-odd-position-of-Array-Java_interview_practice
Java program to print elements at odd position of an array
package oddposition;

/**
 *
 * @author Dinesh Nanda
 */

import java.util.*;

public class OddPostion {

    public static void main(String[] args) {
        
        Scanner s = new Scanner(System.in);
        System.out.println("Enter the size of array: ");
        int size = s.nextInt();
        
        int arr[];
        arr = new int[size];
        
        for(int i = 0; i < size; i++){
            arr[i] = s.nextInt();
        }
        System.out.println("Your entered array is: ");
        for(int i = 0; i < size; i++){
            System.out.print(arr[i]+" ");
        }
        System.out.println();
        System.out.println("Elements at odd position of array is:");
        
        for(int i = 0; i < size; i++){
            if(i%2 != 0){
                System.out.print(arr[i]+" ");           
            }
        }
    }
    
}
