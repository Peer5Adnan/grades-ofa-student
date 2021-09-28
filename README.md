# grades-ofa-student
import java.util.Scanner;
public class Grademar {
    public static void main(String args[]) {
        long j;
        j = 2;
        while (j != 0) {
            int max, min, got;
            max = 500;
            min = 40;
            System.out.println("enter your name");
            String name;
            Scanner n = new Scanner(System.in);
            name = n.nextLine();
            System.out.println("enter your roll no");
            long roll;
            roll = n.nextInt();
            System.out.println("enter marks you have got");
            Scanner g = new Scanner(System.in);
            int tim;
            tim = 5;
            int res;
            res = 0;
            for (int i = 1; i <= tim; i++) {
                got = g.nextInt();
                System.out.println("the marks you have got is for subject " + i + " =  " + got);
                res = res + got;
            }
            System.out.println("marks of the subjects are  " + res);
            if (res == max) {
                System.out.println("you are topper");
            } else if (res >= 375) {
                System.out.println("distiction");
            } else if (res >= 200) {
                System.out.println("pass");
            } else {
                System.out.println("fail");
            }
        }
    }

}
