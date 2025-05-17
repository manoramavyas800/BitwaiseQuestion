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
