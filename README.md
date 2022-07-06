# Lab03ClassroomChaos
Array v ArrayList warmup

# In the src folder is some code
Review the code provided. Answer the following questions by adding comments to your code! You are free to talk with other students, and seek better understanding to these questions. See below for reminders on types, variables, and input

# Step One
Answer the following questions as comments in your code:
1. Why might you want to use an Array instead of an ArrayList?
2. When might our Array not be useful? – need to fill it with more entries, may have way less entries
3. What might we want to use an ArrayList for that we can’t use an Array for?
4. What is the type in Python that most closely resembles an ArrayList?

# Step Two: Coding: recallName(Student s)
As a teacher with likely over 100 students, it's nearly impossible to remember all of their names. Find the method `recallName(Student s)`. 
Write the code for recallName(Student s) to use a **for-loop** do the following:
```
if the Student's name and ID match the name and ID of one of the students in the remembered Array, return the Student's name.
If it isn't in the array or if you have reached a null entry, return "Er...You"
```
**Don't forget to include an if statement that checks for the null, otherwise your program will crash**

For example, if someone calls
```java
  Teacher Steven = new Teacher("src/Students.txt", "src/Memorable.txt");
  Student Jacob = new Student("Jacob", 679);
  Student Adeline = new Student("Adeline", 276);
  Steven.recallName(Jacob);   //Would return "Er...You"
  Steven.recallName(Adeline);   //Would return "Adeline"
```

# Step Three: Test recallName(Student s)
How do you test code? You simply add the lines to your java file (in the future, you will have test lines in separate files).

As such, we would recommend adding the following in main().

```java
Teacher Steven = new Teacher("src/Students.txt", "src/Memorable.txt");
        Student Jacob = new Student("Jacob", 679);
        Student Adeline = new Student("Adeline", 276);
        System.out.println("TESTING " + Steven.recallName(Jacob));
        System.out.println("TESTING " + Steven.recallName(Adeline));
```
Also add your own tests!

# Submitting the Assignment
Make sure to submit the assignment for grading! If you haven't clicked through the canvas link in a while, we would suggest clicking through it again before submitting.

# Reminder on Arrays
Arrays are containers with a set size. Think if them as drawers. You can't just magically make a drawer bigger or smaller once you've made it, it won't fit anymore.
Also, because Arrays have a set size, any entry that doesn't have anything in it will have a "null" entry. Because of this, we have to be careful to not directly try
to read our null entry or we may get some undefined behavior or an error.

# Reminder on ArrayLists
ArrayLists are containers without set sizes. Think of them as bricks. Need a longer wall? Simply add more bricks--your ArrayList will resize to fit everything.
