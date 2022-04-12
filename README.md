# JavaPractice
public class SpeedConverter {
	public static long toMilesPerHour(double kilometersPerHour) {
		if(kilometersPerHour<0) {
			//System.out.println("invalid value");
			return -1;
		}
		//else if(kilometersPerHour>0) {
		// another way to write this is:
		 	//long milesPerHour= Math.round(kilometersPerHour/1.609);
			//return milesPerHour;
			 
			return Math.round(kilometersPerHour/1.609);
		//}
	}
	public static void printConversion(double kilometersPerHour) {
			if(kilometersPerHour<0) {
				System.out.println("Invalid Value");
			}
			else {
			long milesPerHour= toMilesPerHour(kilometersPerHour);
			System.out.println(kilometersPerHour + " km/h = " + milesPerHour + " mi/h ");
		}
	}
	

}
