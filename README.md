# Trailing-zeroes-factorial-

Trailing Zeroes of a factorial 

import java.util.*;

Formula: 

n/5+ n/5^2 + n/5^3+...... 

class Trailingzeroes {

   static int  Tzeroes(int n) {

        int res = 0;

        int powOf5 = 5;

        while (n >= powOf5) {

            res = res + (n / powOf5);

            powOf5 = powOf5 * 5;

        }

       return res;

    }

    public static void main(String... args){

        System.out.println("Enter the value of n: ");

        Scanner sc=new Scanner(System.in);

        int f=sc.nextInt();

        System.out.println("No of trailing zeroes of a factorial number :"+  Tzeroes(f));

    }

}

/*

Enter the value of n:

200

No of trailing zeroes :49

 */
