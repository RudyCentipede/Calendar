import java.text.SimpleDateFormat;
import java.util.Calendar;
import java.util.GregorianCalendar;
import java.util.Scanner;

public class Calendar {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int year = sc.nextInt();
        int month = sc.nextInt();
        int date = sc.nextInt();
        Calendar calendar = new GregorianCalendar(year, month-1, date);
        SimpleDateFormat dateFormat = new SimpleDateFormat("EEEE");
        System.out.println(dateFormat.format(calendar.getTime()));
    }
}
