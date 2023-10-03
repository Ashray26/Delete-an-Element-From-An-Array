//#Delete-an-Element-From-An-Array
import java.util.*;
public class Main
{
  public static void main (String args[])
  {
    int arr[] = { 11, 12, 13, 14, 15, 16, 17, 18, 19, 20 };
    int del_num = 15;
    for (int i = 0; i < arr.length; i++)
      {
	if (del_num == arr[i])
	  {
	    for (int j = i; j < arr.length - 1; j++)
	      {
		arr[j] =arr[j + 1];
	      }
	  }
      }
    for (int i = 0; i < arr.length; i++)
      {
	System.out.print (arr[i] + " ");
      }
  }
}
