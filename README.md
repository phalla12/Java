Java
====
import java.util.Scanner;
public class RandomNumberTest3 {

  
	public static void main(String[] args) {
		Scanner input= new Scanner (System.in);
		RandomNumber user= new RandomNumber();
		int number;
		number= user.GetNumber_1_and_10(20, 30);
		System.out.printf("Random Number:%d",number);
		
	}

}
------------------------------------------
public class RandomNumber {
  public int GetNumber_1_and_10()
	{
		int number;
		number= 1 + (int)(Math.random()*10);
		return number;
	}
  public int GetNumber_1_and_10 (int low, int hi)
  {
	  int number;
	  number= low + (int)(Math.random()*(hi-low));
	  return number;
  }
}
