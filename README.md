import java.util.Scanner;

public class Gpa {

	public static void main(String[] args) {
		System.out.println("How many course you had this semester");
		Scanner sc=new Scanner(System.in);
		int x=sc.nextInt();
		double[] nbcourses=new double[x];
		double sum=0;
		for(int i=0;i<nbcourses.length;i++) {
			System.out.println("Enter your average for the course"+(i+1)+":");
			nbcourses[i]=sc.nextDouble();
		}
		for(int i=0;i<nbcourses.length;i++) {
			sum=sum+nbcourses[i];
		}
		double average=sum/nbcourses.length;
		System.out.println("Average is"+average);
		if(average>90) {
			System.out.println("You have a");
		}
		else if(90>=average && average>80) {
			System.out.println("You have b");
		}
	}

}
