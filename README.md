# max-and-avrg-array
find the highest mark and average mark secured by Hari in "s" number of subjects.
import java.util.Scanner;
public class Exercise1_5{
    public static void main(String[] args) {
	 Scanner input = new Scanner(System.in);
         double mark_avg;
         int result;
         int i;
         int s;
    
       s = input.nextInt();
    
      int[] arr = new int[s];   
      
	 for(i=0;i<arr.length;i++)
	  {
        	arr[i]=input.nextInt();
	  } 
     
int max =arr[0];
   
for( i=1;i<s;i++)
{
  if(arr[i]>max)
  {
    max=arr[i];
  }
}

  
result=max;
System.out.println(result);
  
int sum=0;
for(i=0;i<s;i++)
{
  sum=sum+arr[i];
}
mark_avg = sum/s;
System.out.print(mark_avg);
  
  }
}
