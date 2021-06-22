# Test-Java

public class Main {
    public static void main(String[] args) {
     int[] arr1={1,2,3,4,5};
     int n2= arr1.length;
     rotate(arr1,n2);
     for(int i=0;i<n2;i++){
         System.out.print(arr1[i]+" ");
     }
    }
    public static void rotate(int arr[],int n){
        int temp=arr[n-1];

        for(int i=n-1;i>0;i=i-1){
            arr[i]=arr[i-1];
        }

        arr[0]=temp;
    }
}
