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
		else if(80>=average && average70) {
			System.out.println("You have c");
		}
		else if(70>=average && average>60) {
			System.out.println("You have d");
		}
		else if(60>=average && average>50) {
			System.out.println("You have e");
		}
		else if(50>=average && average>40) {
			System.out.println("You have f");
		}
		else if(40>=average) {
			System.out.println("You have failed,Try next time");
		}
	}

}
