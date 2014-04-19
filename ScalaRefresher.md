riviera-func-spark-lab
======================

Spark hands on lab by Riviera Scala Clojure Meetup (http://www.meetup.com/riviera-scala-clojure).

Objectives
-----------
The objectives of the exercise is a quick refresher of Scala. You will work with Scala list, Tuple, creating functions, and working with 
classes. For those who know Scala very well, you will not need to do this exercise.
You will also write a simple application in Scala as well as working with Scala console. In this exercise, we use Spark console, which is a modified version of Scala Console.


Exercise Set 1
---------------
* Open Spark console.
* Create a list of ten elements: ```(2, 4, 3, 1, 2, 5, 7, 4, 9, 10)``` and assign it to a list ```xs```.
* Create another list ```ys``` containing the double of the list of ```xs```, that is, ```(4, 8, 6, 2, 4, 10, 14, 8, 18, 20)```. Hint: use ```map``` 
* Create another list from ```xs``` , call it ```oddXs```, which contains only the odds number of ```xs```, that is, ```(3, 1, 5, 7, 9)```.
* Group by the element of ```xs``` by its modulo 3. That is: ```( 0 => (3, 9) , 1 => (1, 4, 4, 7, 10), 2 => (2, 2, 5) )``` 
* Sum all elements in element ```xs``` using ```foldLeft```, ```reduce```, or ```sum```
* Compute the average of ```xs```
* Compute the occurence of the each number in ```xs``` using ```map``` and ```reduce```

Exercise Set 2
---------------
* Create a list ```xs``` of integer as follow: ```(1, 1, 4, 3, 5, 2, 5, 6, 1, 7, 8, 9, 2)```.
* Create a list ```ys``` of integer as follow: ```(4, 5, 1, 2, 1, 5, 10, 1, 3, 10, 1, 1, 2)```.
* Create a list ```ts``` of tuples of two elements from ```xs``` and ```ys``` using zip.
 ```( (1, 4), (1, 5), (4, 1), (3, 2), (5, 1), (2, 5), (5, 10), (6,1), (1, 3), (7, 10), (8, 1), (9,1), (2,2))```.
* Create a list ```firsts``` containing only the first element of tuples in the ```ts```, that is, ```(1, 1, 4, 3, 5, 2, 5, 6, 1, 7, 8, 9, 8)```
* Similarly, create ```seconds``` containing only the second element of tuples in the ```ts```.
* Implement a function that receives a list of ```(Int,Int)```, and return another list containing the sum of second elements for each number in 
  the first element. That is: ```( (1, 12), (2, 7), (3, 2), ...)```. Hint: You can use  ```mapValues```
* Create a function mappend(m1:Map[Int,Int], m2:Map[Int,Int]) = Map[Int,Int] that sums the value for the same key and just appends for the key that is not the same. 
