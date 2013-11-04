riviera-func-spark-lab
======================

Spark hands on lab by Riviera Scala Clojure Meetup (http://www.meetup.com/riviera-scala-clojure).

Step 0 - Setup
--------------
* You are expected to have the virtual machine provided by the workshop organizer.
* Make sure that you have spark installed locally:
  * Type ```~/spark-0.8.0/spark-shell``` . Make sure that you have spark shell launched.
  * Type ```val xs = sc.parallelize(List(1,3,5))```
  * And then ```val ys = xs.map(x => x + 1)``` 
  * Quit the shell by typing ```:q``` 
* Make sure you have sbt installed correctly:
  * Type ```sbt```
* Download the starting codes from:
  ```git clone https://github.com/anwarrizal/riviera-func-spark-lab.git```
* Do sanity check by running all the unit tests:
  * Run ```sbt```
  * Then ```test```. All the tests must pass.

Exercises
----------
The exercises we will do during the lab are the following:
* Optional: Quick refresher of Scala
* Exercise 1: Working with spark shell.
* Exercise 2: Word count exercises in shell.
* Exercise 3: Building a stand alone word count application.
* Exercise 4: Implement a simple collaborative filtering application.
* Exercise 5: Implement K means clustering.








