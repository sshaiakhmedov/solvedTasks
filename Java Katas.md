#### 19-Jan

1. A + B

```java
public class FirstClass {
    static byte sum (byte a, byte b) {
        byte c = (byte) (a + b);
       return c;
    }
}
```

2. Opposites Attract
```java
public class OppositesAttract {

  public static boolean isLove(final int flower1, final int flower2) {
return flower1%2==0 && flower2%2==1? true :
flower2%2==0 && flower1%2==1? true : false;
  }
  
}
```

3. Leonardo Dicaprio and Oscars
```java
public class Kata {
  public static String leo(final int oscar){
    if (oscar==88){
    return "Leo finally won the oscar! Leo is happy";
    } else if (oscar==86){
    return "Not even for Wolf of wallstreet?!";
    } else if (oscar==87 || oscar<86){
    return "When will you give Leo an Oscar?";
    } else {
    return "Leo got one already!";
    }
  }
}
```

4. Ghost code?!
```java
public class GhostCode{
  public static String helloName (final String name){
    if (name == null || name.equals("")){
      return "Hello world!";
      } else {
      return "Hello my name is " + name;
      }
  }
}
```

5. Kata Example Twist
```java
public class KataExampleTwist {
    public static String[] kataExampleTwist() {
        String[] websites = new String[1000];
        for (int i=0; i<1000; i++){
        websites[i]="codewars";
        }
        return websites;
    }
}
```

6. Playing with cubes I
```java
public class Cube {
int Side;

public int getSide(){
return Side;
}

public void setSide(int num){
this.Side=num;
}
}
```

7. Lombok Encapsulation
```java
public class EncapsulationDemo{
  private int number;
  private String stringValue;
  private Object anObject;
  
  public EncapsulationDemo (){
  }
  
  public EncapsulationDemo (int number, String stringValue, Object anObject){
  this.number=number;
  this.stringValue=stringValue;
  this.anObject=anObject;
  }
  
  public int getNumber() {
        return number;
    }

    public void setNumber(int number) {
        this.number = number;
    }

    public String getStringValue() {
        return stringValue;
    }

    public void setStringValue(String stringValue) {
        this.stringValue = stringValue;
    }

    public Object getAnObject() {
        return anObject;
    }

```

8. Building blocks
```java
public class Block{
	int width;
  int length;
  int height;
  int volume;
  int surfaceArea;
  
    public Block (int[] array){
    this.width=array[0];
    this.length=array[1];
    this.height=array[2];
    this.volume=width*length*height;
    this.surfaceArea=2*length*height+2*length*width+2*width*height;
    }
    
     public int getWidth() {
        return width;
    }

    public int getLength() {
        return length;
    }

    public int getHeight() {
        return height;
    }
    
    public int getVolume() {
        return volume;
    }
    
    public int getSurfaceArea() {
        return surfaceArea;
    }
```

