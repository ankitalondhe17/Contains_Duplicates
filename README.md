# Contains_Duplicates
Return True if given Array contains Duplicates, return False if not.

//using HashSet

import java.util.HashSet;
import java.util.Set;

public class ContainsDup
{

  public static boolean containsDuplicates(int[] nums)
  {
     Set<Integer> intSet = new HashSet<>();

     for(int num: nums)
     {
        if(intSet.contains(num))
        {
           return true;
         }
         intSet.add(num);
      }
      return false;
  }
  
  public static void main(String[] args)
  
  {
  
    int[] nums = {1,2,3,4,5,1};
    
    System.out.println(containsDuplicates(nums);
    
  }
  
}
