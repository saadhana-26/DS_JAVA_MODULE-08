# Ex12 Add Elements from an Array into a TreeSet
## DATE:23/11/25
## AIM:
To write a Java program that adds elements from an array into a TreeSet and displays the elements in sorted order.
## Algorithm
1. Create an array containing a few integer elements.
2.Create a TreeSet to store elements in sorted order.
3.Use a loop to add each element of the array into the TreeSet.
4.Display the elements of the TreeSet.
5.Stop the Program.
 

## Program:

/*
Program that adds elements from an array into a TreeSet and displays the elements in sorted order.
Developed by: SAADHANA L
RegisterNumber:  212224060224
*/
~~~
import java.util.*;

public class ArrayToTreeSet {

    public static TreeSet<Integer> convertArrayToTreeSet(int[] arr) {
        List<Integer> list = new ArrayList<>();
        for(int x : arr){
            list.add(x);
        }
        
        TreeSet<Integer> treeSet = new TreeSet<>(list);
        return treeSet;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        TreeSet<Integer> treeSet = convertArrayToTreeSet(arr);
        System.out.println("Elements in TreeSet:");
        for (int num : treeSet) {
            System.out.println(num);
        }

        sc.close();
    }
}
~~~

## Output:
<img width="624" height="436" alt="image" src="https://github.com/user-attachments/assets/f4158fec-fadf-438b-b89f-aac3f21fce18" />



## Result:
The program successfully adds elements from an array into a TreeSet.
