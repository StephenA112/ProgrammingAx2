# Programming Fundamentals Assignment2: Pet Day Care Management System

## Name : Stephen Adamson

## Student Number:W20119151


## Chronology of your implementation (what you did first, etc.. )
- The chronological approach followed that laid out in the "Plan of Attack" section of the assignment brief. I started at the 'models' part of the assignment by first creating the Pet and Dog classes. Creating the code for these classes followed the specification to include the infmoration presented in the UML and detailed in the Fields and Consants. Similarly, the Pet class was created following the specifications presented in the Pet tab. Sample values were included in the code as specified but issues were identified later with calling this code.

- I then moved on to create the controllers Daycare and Store.
- Finally I developed the Driver class using the Driver from the previous assignment as a starting point, assisting in the layout and structure of the code presented. This revised updated and expanded to reflect the Driver specification provided.

## Main difficulties you came across in your development of solution and how you solved them.
- In the Pet class, I initially wrote the following code creating a Pet
 ```
  //generate an id
  public Pet(String name, String owner, char sex) {

        this.daysAttending = new boolean[5];
        this.id = nextId;
        nextId++;
        if (name.length() > 30) {
            this.name = name.substring(0, 30);
        } else {
            this.name = "Buddy";
        }
        if (owner.length() > 20) {
            this.owner = owner.substring(0, 20);
        } else {
            this.owner = "Harry Hoover";
        }
        // sex M or F answer
        this.sex = sex;
    }
```
When I ran the Driver and entered a new pet and created a list, the sample fields appeared. This was revised at a later stage and sample fields removed (14-34).
- Having completed the classes and Driver there were a large number of compiling errors found throughout which prevented me compiling the project - an issue experienced in Assignment 1. Reviewing the content identified some simple errors (typos, case sensitive errors) and other issues such as calling incorrect method statements, logic issues, and syntax errors. Some of these were highlighted by IntelliJ and resolved by reviewing course and lab materials.
- 


## Any bugs remaining in the solution or unfinished elements of spec 
- The solution is unfinished and does not include the Cat class, following the message issued on Slack I chose to submit a simplified version of the project.
- The solution does not appear create an XML file in the source folder correctly when the user adds a new pet. I followed instructions from lab 08 on saving and loading to XML files but could not identifiy the error. xstream (v 1.4.20) was downloaded and a lib folder created containing this. As in lab 08 a 'Store' class was created to store this data in XML and code entered into the Driver. As a result the load function on the menu does not return a list.
- 
## Main learnings from your engagement with assignment
Main learnings were the need to take a structured approach to the project - the plan of attack was very useful in guiding the process. Feedback from my first assignment was an important consideration in my approach also. Particularly attention to detail to identify typos, syntax errors etc. this helped direct me.
Source code and final code from other assignments was used and updated, and where necessary using online resources to identify how it could be adapted for this project.
The material still proves challenging to and errors are still present in the code with examples of above components not functioning. Further revision of the materials and labs is required to deepen my understanding of the subject matter that allows me to engage with and produce functional code. 

## Answer the following questions:
     1. Pat Purrs mentioned a problem their friend had with their pet system. What was the issue with that system, and how is your design intended to avoid the same problem?
        All code was written in one large class, no identifiable controller etc., the whole code had to rewritten from scratch. This solution is well structured and formatted with seperate classes, controllers, console driver. This would allow relevant classes to be updated/ amended as required without rewriting the entire code for the project.
     3. Why does Pat want the Driver class to be simple and user-friendly, and how does this relate to the plan to eventually develop a mobile app?
        She wants the code to be simple and well structured to allow transferrability without the need to rewrite it. Simplifying the process by using this as a source code. This will also be beneficial from a UX perspective having a simple menu system.
     4. Pat talked about future expansion of the daycare. What kinds of growth does the system need to support, and how should your code design accommodate this?
        The system should avoid hard coded limits. XML is noted to be useful when storing data in this manner and with this requirement
     6. Besides cats and dogs, what additional animal does Pat plan to include next, and what does this imply for how you structure your inheritance hierarchy?
        Pat plans to include rabbits and other similar animals. The inheritence hierarchy would follow a similar format - rabbit and future animal classes would support the Pet class. A new class would be created for Rabbit, the driver console menu would need to be updated to compile this and update the menu for the user.

## References & Sources
Mandatory : Please list any references used in your development/ implementation of your submission. 
- Java Docs https://www.jetbrains.com/help/idea/javadocs.html
- Java Docs: https://www.oracle.com/europe/technical-resources/articles/java/javadoc-tool.html
- Java Docs: https://www.geeksforgeeks.org/java/java-hello-world-program/
- Driver Class: https://www.geeksforgeeks.org/operating-systems/device-driver-and-its-purpose/
- Increment operators: https://stackoverflow.com/questions/2371118/how-do-the-post-increment-i-and-pre-increment-i-operators-work-in-java
- Instance methods https://www.geeksforgeeks.org/java/instance-methods-in-java/
- Instance methods https://stackoverflow.com/questions/20671008/what-is-the-difference-between-a-local-variable-an-instance-field-an-input-par
- Constructors https://www.geeksforgeeks.org/java/constructors-in-java/
- CRUD explanation https://www.sumologic.com/glossary/crud
- CRUD explanation https://www.geeksforgeeks.org/java/crud-operations-in-student-management-system-in-java/
- Getters and Setters Java: https://www.w3schools.com/java/java_encapsulation.asp
- Getters and Setters https://www.geeksforgeeks.org/java/getter-and-setter-in-java/
- Operators: https://stackoverflow.com/questions/8710619/why-dont-javas-compound-assignment-operators-require-casting?utm
- Casting: https://www.w3schools.com/java/java_type_casting.asp?
- Collections sort: https://docs.oracle.com/javase/tutorial/collections/interfaces/order.html
- XML: https://www.w3schools.com/xml/xml_whatis.asp
- Overriding: https://docs.oracle.com/javase/tutorial/java/IandI/override.html#:~:text=The%20ability%20of%20a%20subclass,the%20method%20that%20it%20overrides.
- Bubble and sorting: https://stackabuse.com/bubble-sort-in-java/
  


Please consider the following statements and choose one (delete the inappropriate one)

- This is my work apart from the specific references noted above (and any code from class notes). I understand the code and can decribe any parts of the solution if needs be;

- This is not all my own work - I'm not sure I understand what I am submitting. 


