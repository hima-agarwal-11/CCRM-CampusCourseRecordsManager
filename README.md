PROJECT OVERVIEW:

CAMPUS COURSE AND RECORDS MANAGER (CCRM)

Heartiest welcome to the CAMPUS COURSE AND RECORDS MANAGER (CCRM), a console-based application which I have built from the root level to help educational institutions manage their academic operations. I learnt about core concepts of Java SE, focusing on building robust , well structured system that handles everything from student enrollment ,  grading system , course managemnt backup and many more. 

I have designed CCRM to be powerful and easy to use using morder highly demanding Java features to ensure that its not just functional but also has a clear demonstartion of strong software design principles.

KEY GEATURES I IMPLEMENTED 

STUDENT HUB:

Easy to add new students, update their details or view their profiles . each and every record is managed with care.

COURSE CATALOG:

Create and manage the course offering , detailings everything from cerdits to the instructor and semester.

SEAMLESS ENROLLMENT:

Enroll and unenroll students in their respective courses ,with the system automatically checking for errors and credit limits .

GRADING AND TRANSCRIPTS:

Record grades and calculate GPAs in no time .Generate detailed academic summary for any student 

DATA PORTABILITY:

I have built a robust import export feature , allowing the user to work with CSV files for easy data exchange .

SAFE AND SOUND:

The automatic backup system creates timestamped snapshots of all your data , so that the user never have to worry about losing progress.

SMART SEARCH :

Quickly find what you need using the search and filter opertations powered by Java's Stream API.

MY TECH STACK AND JAVA JOURNEY:
This project was my space to really learn deep about Java SE. Here's a simple and easy breakdown of what I learned along the way while making this project:
THE EVOLUTION OF JAVA:
A quick look back through journey of java 
* 1991:*
**The Secret Project.** A team at Sun Microsystems starts a secret project called "Oak" to make programming for smart appliances easier.
*1995:*
 **Hello, World! ** The project is renamed **Java** (inspired by coffee) and officially released. Its main idea: "Write Once, Run Anywhere". This means you can
 write code on one computer and it would run on any other, which was a huge deal at the time.
*1996:*
**JDK 1.0.** The first public development kit was released. 
*2004:*
**Java 5 (JDK 1.5): A Big Upgrade.**
This was a huge update that added powerful new features that developers loved.
*2006:* 
**Java Goes Open Source.**
Sun releases Java's core code under an open-source license, letting the community contribute and helping it grow even faster.
*2010:*
**Oracle Takes Over.**
Sun Microsystems is acquired by Oracle.Now, Oracle is the new owner and is in charge of taking care of Java.
*2014:*
**Java 8: The Modern Era Begins.**
This is the most important update since Java 5. It introduced **Lambda Expressions**, which allowed for a much cleaner and more modern style of coding, and the **Stream API** for processing data.
*2018:*
**Faster Releases.** Tired of waiting years for big updates, Oracle changed the release cycle. Now, a new version comes out every six months.
*2019:*
**Java Gets a Price Tag (for some).** Oracle changes its license terms.Java is still free for general personal and development use, but companies now need to pay for updates and support on certain versions from Oracle. 
*2023 and Beyond:*
**Java Today.** Java remains one of the most popular and reliable languages in the world, running on billions of devices. It continues to evolve quickly, adding features to keep it modern, fast, and relevant for huge enterprise applications, cloud systems, and Android development.

PICKING UP THE RIGHT JAVA PLATFORM:
For my project CCRM, I worked with Java SE, because it comes with all the basic tools you need for desktop and server applications.
Java SE(Standard Edition):
Used for general-purpose programming and desktop applications.
Provides core Java libraries: java.lang, java.io, java.util, java.net, etc.
The absolute core of Java. It's the essential toolbox.

Java ME (Micro Edition):
A lighter version made for mobile and small devices.
Targeted at small, resource-constrained devices like mobile phones, set-top boxes, and embedded systems.
Offers a lightweight runtime and a smaller set of APIs than Java SE.
Some new Java SE features (like generics) are often not available.

Java EE (Enterprise Edition, now Jakarta EE)
*A scaled-down version of Java for devices with very limited power, memory, and screen size.
*Made for big enterprise systems with lots of extra libraries.
Built on top of Java SE for large-scale and enterprise-level applications.
*Adds APIs for web services, servlets, JSP, Enterprise Java Beans (EJB), database connectivity, and messaging.
*Ideal for distributed, transactional, and portable server-side applications.
*This format keeps things simple and human-friendly while clearly showing the differences in their use cases and capabilities.

JAVA ARCHITECTURE:

JDK (Java Development Kit): What I used to write and turn my code into bytecode. It comes with the compiler and tools.
*It is everything you need to CREATE and RUN Java programs.
*It's a package that contains:
*The JRE and Development Tools.
*It is neend by  programmer who wants to write and compile code.

JRE (Java Runtime Environment):It is everything you need to RUN a Java program.
*It includes the core libraries and the JVM.
*It is needed by someone who just wants to run a Java program.

JVM (Java Virtual Machine): The engine that actually runs the compiled bytecode on any machine.
*It doesn't understand your original Java code. It only understands a special, compact code called bytecode

They work together write code , compile it into bytecode and then run that bytecode which is executed by the JVM on their specific machine.

HOW TO GET UP RUNNING:

Think of it like this:
I write the code → The JDK turns it into bytecode → Someone else uses the JRE to run it → The JVM makes sure it works on their computer, no matter which operating system they have.

INSTALLATION AND SETUP :
*FOR WINDOWS:
Make sure you have Java JDK 17 or later installed on your machine.
Download the JDK: I have grabbed the latest installer from Oracle's website.
Run the Installer: I just followed the setup wizard's prompts—it was straightforward.
Verify the Installation: I opened Command Prompt and typed java -version and javac -version to confirm everything was installed correctly.
Here is the attached path of the screenshot along with it:
C:\Users\Hima Agarwal\OneDrive\Desktop\CampusCourseRecordsManager\screenshorts
![alt text](javac-version.png.png)
![alt text](jdk-install.png.png)

*RUNNING IN ECLIPSE :


Import the Project: I opened Eclipse, selected File > Import > Existing Projects into Workspace, and browsed to the project folder.


Locate the Main Class: The entry point is in src/edu/ccrm/cli/CCRMApplication.java.
Run the Application: I right-clicked the file and selected Run As > Java Application. The console menu will pop up, and you're ready to go!
![alt text](eclipse-project-structure.png.png)
![alt text](eclipse-run-configuration.png.png)

I have organized the code into clear packages to keep things clean and maintainable like :
edu.ccrm.domain
edu.ccrm.service
edu.ccrm.io
edu.ccrm.cli
edu.ccrm.util
edu.ccrm.config

I have used my acdemic knowledge and brought code into life , I have used it in my code:

*OOP & Inheritance Person (abstract)- Student in the domain package.

*Encapsulation-All fields are private with getters/setters throughout the domain classes.

*Polymorphism-The toString() overrides in Student and Course for display.

*Stream API-CourseService and StudentService for search and filter operations.

*File I/O (NIO.2)-The BackupService class in the io package.

Design Patterns	AppConfig as a Singleton in config, and Course.Builder as a Builder.

*Lambdas Custom comparators in the util.Comparators class.

*Exception Handling-My custom DuplicateEnrollmentException in the exception package.

*Enums Semester and Grade enums in the domain package.

A NOTE ON ASSERTIONS:

I used Java assertions to check important invariants in the code. To run the program with assertions enabled (highly recommended for testing!), use the -ea flag:
bash
java -ea -jar CCRMApplication.jar


SEE IT IN ACTION:
I have included a folder of screenshorts that shows the application from installation process to various features in action. Screenshorts include menu system with options of managing students , courses , backups and many more things.


ACKNOWLEDGEMENT:


This project was an important and memorable learning experience. It has taught me alot. I'd like to thank the Java documentation and various programming communities online that serve as a free sourse to help new begineers like me, they helped me whenever I was stuck .The project 's structure and requirements shapes my academic curiculum , encouraging me to dive deeper into java SE features , exploring them , implementing them and learning them.
