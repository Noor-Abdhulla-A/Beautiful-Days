# Beautiful-Days
# Hackerrank Problem Solution in java

import java.util.Scanner;

public class BeautifulDays {

	public static void main(String[] args) {
		 Scanner in = new Scanner(System.in);
	        int i = in.nextInt();
	        int j = in.nextInt();
	        int k = in.nextInt();
	        int count = 0;
	        
	        for (int a=i;a<=j; a++){
	            StringBuilder temp = new StringBuilder();
	            temp.append(a);
	            temp=temp.reverse();
	            String temp1 = temp.toString();
	            int aRev = Integer.parseInt(temp1);
	            if(Math.abs((a-aRev)%k)==0){
	                count++;
	            }
	        }
	        
	        System.out.println(count);
	    }
	}
