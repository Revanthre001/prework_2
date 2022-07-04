# prework_2
import java.util.Scanner;
class MissingNumberFinder{
    public static void main(String[] args){
        Scanner in = new Scanner(System.in);
        int size = in.nextInt();
        int [] arr = new int[size-1];
        for(int i = 0; i<size-1;i++){
            arr[i] = in.nextInt();
        }
        System.out.println(missingNumberFinder(arr,size));
    }    
    static int missingNumberFinder(int array[], int n){
        int sum;
        sum =((n+1)*n)/2;
        for(int i = 0; i<array.length-1;i++){
            sum-=array[i];
         } return sum;
    }
}
