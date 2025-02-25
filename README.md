# Exercises-using-collection-framework---Date-and-Calendar-class
package userinputdateandcalender;
import java.util.Date;
import java.util.Calendar;
import java.util.Scanner;
public class UserInputDateAndCalender {
 public static void main(String[] args) {
  // Create a Calendar object and set it to the current date and time
Calendar calendar = Calendar.getInstance();
// Print the current date and time using the Calendar object
System.out.println("Current Date and Time: " + calendar.getTime());
// Get the number of days to add from the user
Scanner scanner = new Scanner(System.in);
System.out.print("Enter the number of days to add: ");
int daysToAdd = scanner.nextInt();
// Add the specified number of days to the current date using the Calendar object
calendar.add(Calendar.DAY_OF_MONTH, daysToAdd);
// Get the updated date from the Calendar object
Date updatedDate = calendar.getTime();
// Print the updated date using the Calendar object
System.out.println("Updated Date: " + updatedDate);
//close the scanner to avoid resource leaks
scanner.close();
    }
    
}

Output:

Current Date and Time: Tue Feb 25 15:22:34 IST 2025
Enter the number of days to add: 5
Updated Date: Sun Mar 02 15:22:34 IST 2025

