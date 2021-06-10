* Exercise 3.10

* Is the resulting theory valid or invalid? How many of the tests that pass the precondition also<br> 
pass the postcondition? Explain.
```Java
import org.junit.*;
import org.junit.runner.RunWith;
import static org.junit.Assert.*;
import static org.junit.Assume.*;

import org.junit.experimental.theories.DataPoint;
import org.junit.experimental.theories.DataPoints;
import org.junit.experimental.theories.Theories;
import org.junit.experimental.theories.Theory;

import java.util.*;

@RunWith (Theories.class)
public class ListTheoryTest
{
   @DataPoints
   public static String[] string = {"car", "bike", "train", "plane"};

   @DataPoints
   public static List[] lists = {
      Arrays.asList ("car", "bike", "train"),
      Arrays.asList ("train", "plane", "boat"),
      Arrays.asList ("boat")
   };


   @Theory
   public void removeThenAddDoesNotChangeList
                   (List<String> list, String string)  // Parameters!
   {
      assumeTrue (list != null);            // Assume
      assumeTrue (list.contains (string));  // Assume
      List<String> copy = new ArrayList<String>(list);   // Act
      copy.remove (string);                       
      copy.add (string);
      assertTrue (list.equals (copy));      // Assert
    }
}
```

- So that, the result's theory is definitely invali, because order matters in lists. Plus, the JUnit theory also fails.
