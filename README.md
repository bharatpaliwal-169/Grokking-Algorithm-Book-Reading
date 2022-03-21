# Grokking-Algorithm-Book-Reading

### Chapter - 1
We talk about time complexity and efficiency of a basic algorithm. We study about binary search which on being analised comes out to be the much better option 
as compared to linear search. For example - a 1 bn search would take 1 bn unit if using linear search , where as it will take roughly around < 100 unit time 
which makes binary search almost 15 X better.
Algorithm speed isn’t measured in seconds. Algorithm times are measured in terms of growth of an algorithm i.e in terms of number of operations.

#### travelling salesman problem - one of the worst algo or unsolved programming problem.
Consider a situation where we have a salesman and he have to sell a product in nearby n cities. He wants to travel to all cities and wants to cover minimum distance. Distance amongst 5 cities are given. 

#### solution - 
Now he will find out all the possible paths to travel all the cities, ie all the permuations to travel across the cities. For eg there are 5 cities i.e 120 combo wil be evaluated and the best one i.e the shortest ne would be selected. fr 6 it would be 720 and so on. hence ``` O( n! ) ```.


Code Snippet For Binary Search
```
Given that we have a list of SORTED items.

Let's say we want to search for item X in this list.

low = 0;
high = list.size() - 1; // 0 based indexing

while(low < high){
    mid = (high - low)/2 ;  or mid = (low + high)/2 ; or mid  = low + (high - low)/2;  // we have to choose the mid variation accordingly.
    if(list[mid] > X){
        high = mid - 1;
    }
    else{
        low = mid + 1;
    }
}

Return the IDx of the required element.

```


-----------------------------------------------------------------------------------------------------------------------------------------------------------

### Chapter - 2 : Sorting Algos



Understanding the pros and cons of using Arrays and Linked List , according to the need of usecase. If we need a lot of random access array is goto DS, if CRUD is priority LL is more prefered.

