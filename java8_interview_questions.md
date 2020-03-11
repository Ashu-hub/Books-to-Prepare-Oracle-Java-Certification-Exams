
# Java 8
1. List all Java 8 Features  
2. What are defender methods and why they were introduced in Java?   
3. How diamond problem is avoided in Java after addition of Interface as a class can implement any number of Interface?  

4. Relation between Functional Interface and Lambda expressions?  
5. Lambda is implemented at Compiler level or JVM level?  
6. Functional Interfaces added by Java in java.util.function with their use?  
7. lambda expression use and code?  
8. Functional Interface, give example of Runnable, Comparator?  

9. Stream api and any use case?  
10. collectors in java 8?  
11. distinct, sort and frequency example?      

# Java 8 Answers
**1. List all Java 8 (Released 18th March 2014) Features**  

       a. default and static methods in Interface  
       b. Lambda Expression and Functional Interfaces  
       c. forEach() method in all Collections (via static method in Iterable Interface)  
       d. Streams for Bulk data operation on Collections  
       e. Date time API (based on Joda Time)  
       f. Memory space and garbage collection improvement  
       g. Comparator interface with lot of util metods  
       h. performance improvement in Map
   
**2. What are defender methods and why they were introduced in Java?**  
   **Default/Defender/Virtual extension method:**  
     default methods in Interface were allowed to make changes to the existing API without actually breaking them.
     If we see Collections API, Same Interface has been implemented by many implementations, adding even a single method in interfaces results in breaking all the existing implementing classes. default method came to rescue here that lets defining the default implementation at one place which will be available for all implementations.  
     **e.g.:** `forEach()` and `spliterator()` methods added to `java.lang.Iterable`. Because of this change, these methods are available in all the collection API implementing Iterable.  
     **Ref:** https://dzone.com/articles/introduction-default-methods
   
   **static methods:**  
     These methods are same as static methods in Class.  
     Use: Create a Utility Interface instead of class having all the static methods, as anyway you do not need to initialize the class having all the static methods.  
   
**3. How diamond problem is avoided in Java after addition of Interface as a class can implement any number of Interface?**  
    
	
**4. Relation between Functional Interface and Lambda expressions?**  

**5. Lambda is implemented at Compiler level or JVM level?**  
Ref: https://stackoverflow.com/questions/29143803/java-lambdas-how-it-works-in-jvm-is-it-oop  
     https://blog.overops.com/compiling-lambda-expressions-scala-vs-java-8/  

	