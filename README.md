# Exercises-using-collection-framework---Date-and-Calendar-class
package userinputdateandcalendar;
import java.util.Date;
import java.util.Calendar;
import java.util.Scanner;
public class UserInputDateAndCalendar {
    public static void main(String[] args) {
        // TODO code application logic here
        Calendar calendar = Calendar.getInstance();
        System.out.println("Current Date and Time: " + calendar.getTime());
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the number of days to add: ");
        int daysToAdd = scanner.nextInt();
        calendar.add(Calendar.DAY_OF_MONTH, daysToAdd);
        Date updatedDate = calendar.getTime();
        System.out.println("Updated Date: " + updatedDate);
        scanner.close();
    }
}
Output
Current Date and Time: Tue Feb 25 15:55:21 IST 2025
Enter the number of days to add: 5
Updated Date: Sun Mar 02 15:55:21 IST 2025
