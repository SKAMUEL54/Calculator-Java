import java.util.*;

//Simple calculator

public class Main
{
    public static void main(String[] args)
    {
        Scanner in = new Scanner(System.in);
        double a, b, c;

        System.out.print("Enter the first number \n");
        a = in.nextDouble();
        System.out.print("And enter second  \n");
        b = in.nextDouble();
        System.out.print("""
                Choose the operation \s
                1.Addition
                2.Subtraction
                3.Multiplication
                4.Division
                5.Power
                #Please enter the number of operation\s
                """);
        double somethin = in.nextDouble();
        double addition = 1;
        double subtraction = 2;
        double multiplication = 3;
        double division = 4 ;
        double power = 5;
        if (somethin == addition) {
            c = a + b;
            System.out.println(a + " + " + b + " = " + c);  }
        else if (somethin == subtraction)  {
            c = a - b;
            System.out.println(a + " - " + b + " = " + c);	}
        else if (somethin == multiplication)	{
            c = a * b;
            System.out.println(a + " * " + b + " = " + c);	}
        else if (somethin == division)   {
            c = a / b;
            System.out.println(a + " / " + b + " = " + c);	}
        else if (somethin == power)	{
            System.out.println("""
                    Enhance A or B?
                    1.A
                    2.B""");
            double enhance = in.nextDouble();
            double first = 1;
            if (enhance == first) {
                System.out.println(Math.pow(a, 2)); }
            {
                System.out.println(Math.pow(b, 2)); }

        }
    }
}
