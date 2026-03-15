# Ex14 Tracking the First Unique Number in a Stream using LinkedHashMap
## Date: 11.2.26
## AIM:
To implement a program that tracks the first unique (non-repeating) number in a stream of integers using a LinkedHashMap.

## Algorithm
1.Maintain a LinkedHashMap to store each number and its frequency.

2.For every incoming number, update its count in the map.

3.After each update, scan the map in insertion order.

4.The first key having frequency 1 is the current first unique number.

5.If no such key exists, print “No unique number”.  

## Program:
```
/*
Program to tracks the first unique (non-repeating) number in a stream of integers using a LinkedHashMap.
Developed by: Sri Yaline R
RegisterNumber: 212224040325
```
```
import java.util.*;

public class FirstUniqueNumberStream {

    public static void processStream(int n, Scanner sc) {
        
    LinkedHashMap<Integer,Integer> hm =new LinkedHashMap<>();
    for(int i=0;i<n;i++){
        int a=sc.nextInt();
        Integer unq=null;
        hm.put(a,hm.getOrDefault(a,0)+1);
        for(Integer key:hm.keySet()){
            if(hm.get(key)==1){
                unq=key;
                break;
            }
        }
        if(unq!=null){
            System.out.println("First unique number: "+unq);
        }
        else{
            System.out.println("No unique number");
        }
        
    }
    
    
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        processStream(n, sc);
        sc.close();
    }
}
  
*/
```

## Output:
<img width="773" height="537" alt="image" src="https://github.com/user-attachments/assets/ff5a5d01-5ec1-410c-93a8-e1fdd52fd12b" />


## Result:
The JAVA program successfully tracks and returns the first unique number at any point in the integer stream using a LinkedHashMap.
