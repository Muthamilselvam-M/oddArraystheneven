# oddArraystheneven
import java.util.Arrays;
public class Main
{
	public static void main(String[] args) {
		System.out.print("Enter the length of the array:");
		Scanner a = new Scanner(System.in);
		int input = a.nextInt();
		int[] arr = new int[input];
		System.out.println("Enter the array element:");
		for(int i=0;i<input;i++){
		int input1 = a.nextInt();
		arr[i]=input1;
		}
		System.out.println("The array is: "+ (Arrays.toString(arr)));
		new1(arr);
}
	public static void new1(int[] arr){
	    int j = arr.length-1;
	    int k=0;
	    int[] arrayNew = new int[arr.length];
	    for(int i=0;i<arr.length;i++){
	        if (!(arr[i]%2==0)){
	            arrayNew[k++]=arr[i];}
	            
	        else
	            
	            arrayNew[j--]=arr[i];
	    }
	        System.out.println("The odd arrays are: "+ (Arrays.toString(arrayNew)));
	     
	    
	}
}
