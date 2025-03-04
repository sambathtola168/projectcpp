
import java.util.Scanner;

public class Main {
    
static void  Sort(float arr[],int n){ 
    float tmp;
    for(int i=0;i<n;i++){
        for(int j=i+1;j<n;j++){
            if(arr[i]<arr[j]){
                tmp=arr[i];
                arr[i]=arr[j];
                arr[j]=tmp;
            }
        }  
        
    
    
}
    }
static void input(float arr[],int n){
    Scanner sc=new Scanner(System.in);
        for(int i=0;i<n;i++){
            System.out.println("input number "+(i+1)+" : ");
          arr[i]=sc.nextFloat();
        }
    }
    
    static void output(float arr[],int n){
        for(int i=0;i<n;i++){
            System.out.print(arr[i]+" ");

        }
    }

    
  public static void main(String[] args) {
      int n;
      Scanner sc =new Scanner(System.in);
      System.out.println("Input n element : ");
      n=sc.nextInt();
      float arr[]=new float[n];
      input(arr,n);
      output(arr,n);
      Sort(arr,n);
     output(arr,n);
      
  }
}
