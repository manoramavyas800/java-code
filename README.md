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
