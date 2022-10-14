###  [Task 8kyu](https://www.codewars.com/kata/54edbc7200b811e956000556/train/java)


Consider an array/list of sheep where some sheep may be missing from their place. We need a function that counts the number of sheep present in the array (true means present).





### My solution
```Java
     public class Counter {
    public int countSheeps(Boolean[] arrayOfSheeps) {
        int c=0;
        for(int i=0; i<arrayOfSheeps.length; i++){
            if (arrayOfSheeps[i]==null){continue;}
            if(arrayOfSheeps[i]==true){
                c++;
            }

        }

        return c;
    }
}
```

### Fav solution
```Java
import java.util.Arrays;
import java.util.Collections;

public class Counter {
public int countSheeps(Boolean[] arrayOfSheeps) {
return Collections.frequency(Arrays.asList(arrayOfSheeps), true);
}
}

```
I like this solution because I like it
