### Task 8 kyu

[Task link](https://www.codewars.com/kata/54edbc7200b811e956000556/)

Consider an array/list of sheep where some sheep may be missing from their place. We need a function that counts the number of sheep present in the array (true means present).

### My solution

```Java

public class Counter {
    public int countSheeps(Boolean[] arrayOfSheeps) {
        int counter = 0;
        for(Boolean b : arrayOfSheeps){
            try{
                if(b.equals(true))
                    counter++;

            }catch(Exception e){}
        }
        return counter;
    }
}

```

### Favourite solution from code-wars

```Java

public class Counter {
    public int countSheeps(Boolean[] arrayOfSheeps) {
        // TODO May the force be with you
        int total = 0;
        for (Boolean arrayOfSheep : arrayOfSheeps) {
            if (arrayOfSheep == null) continue;
            if (arrayOfSheep == true) total += 1;
        }
        return total;
    }
}

```

Interesting construction, I have learnt some from it.

# Have a nice day!