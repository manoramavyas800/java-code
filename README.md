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
