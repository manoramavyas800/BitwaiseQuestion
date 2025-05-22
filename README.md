# BitwaiseQuestion
//Count bitset (count how many 1 in these number)

public class CountBit {
    public static void main(String[] args) {
        int count=0;
        int n=5;
        while(n!=0) {
            if ((n & 1) == 1) {
                count++;
            }
            n = n >>1;
        }
        System.out.println(count);
    }
        }
    //Count kth bit (if kth bit is 1 print is bit)
    import java.util.Scanner;
public class FindKthBit {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int count=0;
        int n=sc.nextInt();
        int k=sc.nextInt();
        if(((n>>(k-1))&1)==1){
            count++;
        }

        System.out.println(count);
    }
        }
//chack given number is power of two or not

import java.util.Scanner;
public class ChackPower {
          public static void main(String[] args) {
              Scanner sc = new Scanner(System.in);
              int n = sc.nextInt();
              boolean isBitset=true;
              while(n!=1) {
                  if ((n & 1) != 0) {
                      isBitset = false;
                      break;
                  }
                  n >>= 1;
              }
                  System.out.println(isBitset ? "YES" : "NO");

          }
          }

    //FIND THE FREQUENCY BY USING THE BITWISE OPERATOR IN WHICH TWO NUMBERS ARE COMING AT ODD TIME.

    public class Frequency {
    public static void main(String[] args) {
        int arr[] = {3, 4, 3, 4, 5, 4, 4, 6, 7, 7};
        int n = arr.length;
        int res1 = 0;
        int x = 0;
        int res2 = 0;
        for (int i = 0; i < n; i++) {
            x ^= arr[i];
        }
        int k = x & (x - 1);
        for (int j = 0; j < n; j++) {
            if ((k & arr[j]) == 0) {
                res1 = res1 ^ arr[j];
            } else {
                res2 = res2 ^ arr[j];
            }
        }
        System.out.println(res1);
        System.out.println(res2);
    }
}

// FIND THE FREQUENCY BY USING THE BITWISE OPERATOR IN WHICH ONE NUMBERS IS COMING AT ODD TIME.

public class Codeforces {
    public static void main(String[] args) {
        int[] arr = {3, 4, 3, 4, 5, 4, 4, 7, 7};
        int n = arr.length;
        int res1 = 0;
        int x = 0;
           for (int j = 0; j < n; j++) {
               if ((x & arr[j]) == 0) {
                   res1 = res1 ^ arr[j];
               }
           }
       
        System.out.println(res1);

    }

}
