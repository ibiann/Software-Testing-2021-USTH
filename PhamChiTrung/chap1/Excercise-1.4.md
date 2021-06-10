# Excercise 1.4 #

## a) 
```Java
import java.util.Vector;

class Vector_test {
    public static Vector union (Vec a, Vec b) {
        Vec v = new Vector();
        v.addAll(a);
        v.addAll(b);
        return v;
    }
    public static void main(String[] args) {
        Vec a = new Vector();
        a.add(10);
        Vec b = new Vector();
        b.add(8);
        Vec v = union(a, b);
    }
}
```

## b) lack of verification statements such as checking the two vectors are empty or have different dimensions.

## c) TestCase
```Java
Vector a = new Vector()
Vector b = new Vector()
```
```Java
Vector a = new Vector();
a.add(10)
Vector b = new Vector();
```
```Java
Vector a = new Vector();
Vector b = new Vector();
b.add(8)
```

## d) TestCase
```Java
public static Vector union(Vector a, Vector b, boolean inv = False)
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
      return v;
    }
  }
}
```
        
