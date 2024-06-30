import java.util.Scanner;
public class CalculateStudentGrades {
    public static void main(String args[]) {
        float sum=0;
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter number of subjects::");
        int subject = sc.nextInt();
        System.out.println("Enter Maximum marks::");
        int max = sc.nextInt();
        
        for (int i=1;i<=subject;i++) {
            System.out.println("Enter marks of "+i+" subject:");
            float marks = sc.nextFloat();
            if(marks>max){
                for(float j=marks;j>max;j=j+0){
                    System.out.println("Invalid mark, please enter valid mark:");
                    marks = sc.nextFloat();
                    j=marks;
                }
            }
            sum = sum + marks;
        }
        int total = max*subject;
        System.out.println("Total marks you obtained out of "+total+" are: "+sum);
        
        float average;
        
        average = (sum/total)*100;
        System.out.println("Average percentage:"+average+"%");
        char grade;

        if(average>=80){
            grade = 'A';
        }else if(average>=60 && average<80){
            grade = 'B';
        }
        else if(average>=40 && average<60){
            grade = 'C';
        }
        else {
            grade = 'D';
        }
        System.out.println("Your grade is " + grade);
        switch(grade) {
            case 'A' :
                System.out.println("Excellent!");
                break;
            case 'B' :
                System.out.println("Good");
            case 'C' :
                System.out.println("Well done");
                break;
            case 'D' :
                System.out.println("You passed");
            case 'F' :
                System.out.println("Better try again");
                break;
            default :
                System.out.println("Invalid grade");
        }
    }
}
