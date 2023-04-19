# Switch-Method
#Determine Week Day: input - number of day 0 (Sunday) to 6 (Saturday) - return if the day is a Week Day.
#Determine Name Of Month: input - number of month 1 (January) to 12 (December) - output - Name of Month.
#Determine Name Of Day: input - number of day 0 (Sunday) to 6 (Saturday) - return the day of week in text.

-------------------------------------------------------------------------------------------------------------
package ifstatement.examples;

public class SwitchExercisesRunner {

	public static void main(String[] args) {
		System.out.println(determineNameOfDay(1));
		System.out.println(determineNameOfMonth(6));
		System.out.println(isWeekDay(6));
	}

	public static boolean isWeekDay(int dayNumber) {
		switch (dayNumber) {
//		case 0:
//		case 6:
//			return false;
		case 1:
		case 2:
		case 3:
		case 4:
		case 5:
			return true;

		}
		return false;
	}

	public static String determineNameOfDay(int dayNumber) {
		switch (dayNumber) {
		case 0:
			return "Sunday";
		case 1:
			return "Monday";
		case 2:
			return "Tuesday";
		case 3:
			return "Wednesday";
		case 4:
			return "Thursday";
		case 5:
			return "Friday";
		case 6:
			return "Saturday";
		}
		return "Invalid_day";

	}
	
	public static String determineNameOfMonth(int monthNumber) {
		switch (monthNumber) {
		case 1:
			return "January";
		case 2:
			return "February";
		case 3:
			return "March";
		case 4:
			return "April";
		case 5:
			return "May";
		case 6:
			return "June";
		case 7:
			return "July";
		case 8:
			return "August";
		case 9:
			return "Septemper";
		case 10:
			return "Octorber";
		case 11:
			return "November";
		case 12:
			return "December";
		}
		
		return "Invalid_month";
	}
		
}
