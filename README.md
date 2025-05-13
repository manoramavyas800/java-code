# java-code
//count primeFectorial
import java.util.Scanner;
public class PrimeNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        System.out.print("1 ");
        int CountNum=1;
        for(int i=2;i<=n;i++){
            while(n%i==0){

                CountNum=i;
                n=n/i;
                System.out.print(CountNum+" ");
            }
        }
    }
}



//find max num in array

public class findMaxNum {
    public static void main(String[] args) {
        int [] arr = {2,4,5,6,7};
        int ans=arr[0];
        for (int i = 1; i < arr.length; i++) {
            if(arr[i]>ans){
                ans=arr[i];

            }
        }
System.out.println(ans);

    }
       }

       //print these patterns
       /*
       1 
       1 2 
       1 2 3 
       1 2 3 4 
       1 2 3 4 5 */

       import java.util.Scanner;
public class Java {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter number");
        int n=sc.nextInt();
        for(int i = 1; i <=n; i++) {
            for (int j = 1; j <= i; j++) {
                System.out.print(j+" ");
            }
            System.out.println();
        }
        }
    }

    //chack Number is palindrome or not

    import java.util.Scanner;
public class Palindrome {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int num = sc.nextInt();
        int revesse=0;
        int temp=num;
        while(temp!=0){
            int rem=temp%10;
            revesse=revesse*10+rem;
            temp=temp/10;
        }
        if(revesse==num){
            System.out.println("Palindrome Number");
        }else{
            System.out.println("Not a Palindrome Number");
        }
}
}

//print Fectorial in java

import java.util.Scanner;
public class Fectorial {
    public static int Fectorial(int n) {
        int xFect = 1;
        for (int i = 1; i <= n; i++) {
            xFect *= i;
        }
        return xFect;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
            System.out.println(Fectorial(n));
    }
}

//Seive Eratosthenes Theorm to find prime number in given range n

import java.util.Scanner;
public class java {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
       boolean [] isPrime = new boolean[n+1];
        for (int i = 2; i <= n; i++) {
            isPrime[i] = true;
        }
        for (int j = 2; j*j <=n; j++) {
            if (isPrime[j]) {
                for(int i=j*j; i <=n; i+=j) {
                    isPrime[i] = false;
                }
            }
        }
        for (int i = 2; i <= n; i++) {
            if(isPrime[i]) {
                System.out.println(i+" ");
            }
        }
    }
}
