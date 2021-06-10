# Excercise 1.4 #

## Write a Java method with the signature
```Java
import java.util.Vector;

class Vec_test {
    public static Vector union (Vector a, Vector b) {
        Vec v = new Vector();
        v.addAll(a);
        v.addAll(b);
        return v;
    }
    public static void main(String[] args) {
        Vector a = new Vector();
        a.add(10);
        Vector b = new Vector();
        b.add(8);
        Vector v = union(a, b);
    }
}
```

## 
One of possible fault is lack of verification statements such as checking the two vectors is having different dimensions.

##
```Java
public static Vector union(Vec a, Vec b)
{
  if (a.isEmpty() && b.isEmpty()) return Null;
  else
  {
    if (inv)
    {
      Vec v = new Vector();
      v.addAll(b);
      v.addAll(a);
      return v;
    }
    else
    {
      Vec v = new Vector();
      v.addAll(a);
      v.addAll(b);
    }
  }
}
```
