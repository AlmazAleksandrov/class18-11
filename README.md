### Task 8kyu:

You are given two interior angles (in degrees) of a triangle.
Write a function to return the 3rd.
Note: only positive integers will be tested.

[Task link](https://www.codewars.com/kata/5a023c426975981341000014/train/java)

#### Solution:
```
public class ThirdAngle {
    public static int otherAngle(int angle1, int angle2) {
        return (180 - angle1 - angle2);
    }
}
```

#### Fav solution:
```
public class ThirdAngle {
    public static int otherAngle(int angle1, int angle2) {
        int angle3;
        if(angle1<0 || angle2<0){
           System.out.println("Only positive integers!");
           }
        angle3 = 180 - (angle1+angle2);
        if(angle3<0){
        System.out.println("Impossible!");
        }
        return angle3;
    }
}
```

#### Comment:
Well done did the angle check, although it was possible without it.


### Task 7kyu:

Trolls are attacking your comment section!
A common way to deal with this situation is to remove all of the vowels from the trolls' comments, neutralizing the threat.
Your task is to write a function that takes a string and return a new string with all vowels removed.

[Task link](https://www.codewars.com/kata/52fba66badcd10859f00097e/train/java)

#### Solution:
```
public class Troll {
  public static String disemvowel(String str) {
      return str.replaceAll("[AaEeIiOoUu]", "");
  } 
}
```

#### Fav solution:
```
public class Troll {
  public static String disemvowel(String str) {
      return str.replaceAll("[AaEeIiOoUu]", "");
  } 
}
```

#### Comment:
I like my own solution the most, the others were not impressed.
