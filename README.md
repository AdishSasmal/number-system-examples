import java.text.NumberFormat;

//13NOV2020
//Formatting of numbers 
//Number class 
//Methods 
//void setMaximumFractionDigits(int val)
//void setMinimumFractionDigits(int val)
//void setMaximumIntegerDigits(int val)
//void setMinimumIntegerDigits(int val)

public class ex22 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		
		double pay = 171.06890744956786;
		//create an object of NumberFormat class using NumberFormat.getInstance
		NumberFormat ob=NumberFormat.getInstance();
		//set no digits on fraction part round to nearest cent.
		ob.setMinimumFractionDigits(2); //atleast 2 nos
		ob.setMaximumFractionDigits(5);//limit to 5 places
		//Format pay call format(double d)
		System.out.println(ob.format(pay));

	}

}
