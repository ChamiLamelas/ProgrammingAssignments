# Programming Assignments

In this file, I describe the assignments I either created or rewrote during my time as a teaching assistant at Brandeis University. Descriptions of the assignments I created are included in this repository. For more information about these assignments such as access to the starter code, solutions, or tests please contact me at either slamelas@brandeis.edu or Swaminathan.Lamelas@tufts.edu. For the assignments I rewrote, you can contact me as well.

## Assignments Created

For assignments that I created, I came up with the idea and set up entirely. The only information I started with was which topics (usually which data structures) the assignment should cover.

### Text Editor

**Course:** COSI 21a Data Structures and the Fundamentals of Computing

**Goal:** Have students implement a doubly linked list from scratch and use it in an application.

**Semesters Used:** 2

This assignment has students implement a simple text editor using a modified doubly linked list (DLL). The editor supports character insertion and deletion as well as cursor movement forwards and backwards across the editor. For this assignment:

* I came up with the idea of applying a doubly linked list to implementing a text editor.
* I wrote the assignment description file. This introduces students to how they will be building the modified DLL that backs the text editor which includes managing a cursor. 
* I prepared a starter kit with a skeleton file for the modified DLL as well as files that allow students to see a GUI version of the editor that uses the students work to hold the editor text and perform character manipulation.
* I implemented my own solution from scratch that is tested with a large suite of JUnit tests which I wrote that are also used for grading students' code.

### Worktime Analysis

**Course:** COSI 21a Data Structures and the Fundamentals of Computing

**Goal:** Have students implement a splay tree from scratch and use it in an application.

**Semesters Used:** 2

This assignment has students implement a system for analyzing work entries by an employee that is built on a modified splay tree. The tool allows users to search for work entries based on their title with the idea being that an employee may not always title the same activity the same. For instance, if someone is interested in how much time an employee spends on grading, the employee may log grading activities with a variety of titles that the employer may try to look up in succession such as "grading", "grading homework", "grading quizzes", "graded homework", etc. A splay tree is used as it takes advantage of locality-based searches. For this assignment:

* I came up with the idea of applying a splay tree to worktime analysis.
* I wrote the assignment description file. This introduces students to how they will be implementing this system via a modified splay tree. The system also includes a simple read-eval-print-loop where users can search and remove work entries.
* I prepared a starter kit with skeleton files for all the files students implement as well as some starter code that loads in some sample work entry data that I prepared myself.
* I implemented my own solution from scratch that is tested with a large suite of JUnit tests which I wrote that are also used for grading students' code.

### Spam or Safe?

**Course:** COSI 21a Data Structures and the Fundamentals of Computing

**Goal:** Have students implement a closed hashing hash table and binary heap based priority queue from scratch and use them in an application.

**Semesters Used:** 1

This assignment has students implement a system for detecting spam emails using a modified hash table and priority queue. The tool is trained on batches of emails that have been labelled as spam or not by hand. The tool will receive batches of unlabelled emails to filter and new training batches that will be used to update the spamicity of emails that are stored (in an inbox). For this assignment:

* I came up with the idea of applying a hash table and priority queue to solving the problem of email filtering.
* I wrote the assignment description file. This introduces students to how they will be implementing this system via a modified priority queue and hash table. This includes explaining how the spamicity of a word will be calculated; the spamicity of a word is the probability of an email containing that word being spam.
* I prepared a starter kit with skeleton files for all the files students implement as well as some starter code that loads in labelled and unlabelled emails that I prepared myself.
* I implemented my own solution from scratch that is tested with a large suite of JUnit tests which I wrote that are also used for grading students' code.

## Assignments Rewritten

For assignments that I wrote, I used an existing idea to rebuild the assignment. This was typically motivated by the need to clarify aspects of the assignment or make them testable for more objective, and therefore fair, grading.

### Elevator

**Course:** COSI 21a Data Structures and the Fundamentals of Computing

**Goal:** Have students implement a simulation that involves a variety of classes that interact with each other.

**Semesters Used:** 2

This assignment has students implement a simulation of an elevator that moves up and down and services clients in a first-come-first-serve fashion. The elevator services people who have a destination floor to travel to from the lobby. I did not come up with the idea of having an elevator simulation to test students' knowledge of object oriented programming, but I ended up writing up the assignment from scratch to make it more clear for students and more easily testable for grading. For this assignment:

* I wrote the assignment description file. This introduces students to how exactly the elevator will work and how the various classes should interact with each other.
* I prepared a starter kit with skeleton files for all the files students implement.
* I implemented my own solution from scratch that is tested with a large suite of JUnit tests which I wrote that are also used for grading students' code.

### Unix Shell Part 1 & 2

**Course:** COSI 131a Operating Systems

**Goal:** Have students become familiar with the pipes and filters design pattern as well as multithreading in Java.

**Semesters Used:** 1

This assignment has students implement a simplified Unix shell that allows the user to execute common Unix commands via Java's interface with the file system. Students implement this using the pipes and filters design pattern where the filters (i.e. subcommands) are executed sequentially in part 1 and concurrently using Java threads in part 2. An older version of this assignment had been used at Brandeis in Operating Systems for sometime, but Eitan Joseph and I rebuilt this assignment. For this assignment:

* We wrote the assignment description file. This introduces students to what aspects of the shell need to be implemented and how they will be doing so using the pipes and filters design pattern.
* We prepared a starter kit with skeleton files for all the files students implement as well as some starter code for the pipes.
* We implemented separate solutions from scratch that are tested with a large suite of JUnit tests that are also used for grading students' code. Many of the tests were taken from an older version of this assignment written by Ryan Marcus but we also added more.

### Cars and Tunnels Part 1 & 2

**Course:** COSI 131a Operating Systems

**Goal:** Have students become familiar with some of the aspects of CPU process scheduling.

**Semesters Used:** 1

This assignment has students simulate CPU process scheduling by scheduling vehicles travelling through tunnels. Vehicles serve as an abstraction of processes that require tunnels that abstract CPU cores where vehicles can perform their task (driving). Students use a variety of synchronization mechanisms to practice concepts such as locking, conditions, and mutual exclusion to implement the scheduling efficiently. An older version of this assignment had been used at Brandeis in Operating Systems for sometime, but Eitan Joseph and I rebuilt this assignment. For this assignment:

* We wrote the assignment description file. This introduces students the policy of the scheduler and how it needs to be implemented (e.g. to avoid busy waiting).
* We prepared a starter kit with skeleton files for all the files students implement as well as some starter code for how vehicles drive.
* We implemented separate solutions from scratch that are tested with a large suite of JUnit tests that are also used for grading students' code. Some of the tests were taken from an older version of this assignment and some are new ones we wrote.