Download Link: https://assignmentchef.com/product/solved-csci203-part-b-in-java
<br>
Your task for this assignment is to investigate some of the properties of queues.

You should write a Java or C++ program which simulates the queuing and service of a set of requests at a fast food restaurant.

Input consists of the following data:

<ul>

 <li>The number of primary servers in the system.</li>

 <li>The number of secondary servers in the system.</li>

 <li>A set of service requests each consisting of an arrival time and two service times. This set is terminated by a dummy record with arrival time and service times all equal to 0. (Note: the arrival times are sorted in ascending order).</li>

</ul>

For example, the data file:




3 2

1 2 3

3 3 5

<ul>

 <li>2 2</li>

 <li>3 2</li>

 <li>2 4</li>

</ul>

0 0 0




indicates there are 3 primary servers and 2 secondary servers. The first service (customer) arrives in minute 1 (first minute of simulation), and the service requires 2 minutes of primary server’s time and 3 minutes of secondary server’s time. The second service (customer) arrives in minute 3, and it requires 3 minutes of primary server’s time and 5 minutes of secondary server’s time, etc.




The last entry of the data file 0 0 0 indicate the end of simulation. (Note that it is possible to have two customers arrive in the same time as shown in the above sample data (second and third customers).)




Your program should read the name of the data file from standard input and then read the data in the named file into the simulation. For example, the following command will trigger the execution of your program by reading the data file provided:




./QueueSim datafile.dat     or




java QueueSim datafile.dat




The simulation is to be of a system with two sets of servers, primary and secondary, with a single queue associated with each set. Customers arrive in the system and are served first by a primary server and, on completion of this service, by a secondary server. If all servers of a particular type are busy, the customer will enter either the primary or secondary queue as appropriate.




The simulation should be run until the last customer has left the system.




Output, to standard output, for each version of the queuing process will consist of the following data:

<ul>

 <li>Number of people served.</li>

 <li>Time last service request is completed.</li>

 <li>Average total service time.</li>

 <li>Average total time in queue(s). Both overall and separate.</li>

 <li>Average length of queue. For each queue and overall.</li>

 <li>Maximum Length of queue. For each queue and overall.</li>

 <li>Total idle time for each server.</li>

</ul>







Other requirements:

<ul>

 <li>Software (programming language):

  <ul>

   <li>Java Version – JDK 6 update 17 or above (Using Windows) o C++ / C compiler – g++ 4.0 or above (Using Linux)  Operating System:</li>

   <li>Windows XP Professional, o Windows Vista Home / Business,  o Windows 7,  o Windows 10, o Ubuntu Linux 8.04 LTS or above.</li>

  </ul></li>

 <li>If you use a different environment, please make sure that you MUST check with your lecturers first!</li>

 <li>For C++ solution, students are to give batch / make files for compilation.</li>

 <li>Students are to place all compilation and instructions on how to run the program inside a <strong>txt</strong> file. The markers will refer to this file when marking.</li>

</ul>

Programs should be appropriately documented with comments.







NOTE: Since the question is to assess your understanding of the concept of Queue, you are NOT allowed to use the library of the language that implement queue. You need to write the codes (implementation) of Queue for this exercise. (See point (iii).)







Sample output:




YCT-MacBook:csci203 sionggojapit$ ./a2 a2data6.txt

Simulation Start Time: Sat Jul 24 02:41:39 2021




a2data6.txt is used for this simulation.

Start simulation using filename -&gt; a2data6.txt

This simulation uses 6 primary server(s), and 6 secondary server(s).




Total minute of simulation: 277

Number of people served: 100




Total service time: 1888

Average total service time: 18.88 minutes




Average total time in primary server queue: 1 minutes

Average total time in secondary server queue: 0.966667 minutes

Average total time in both queue: 0.983333 minutes




Total primary queue size: 3

Total secondary queue size: 60




Average length of primary queue: 0.0108303

Average length of secondary queue: 0.216606

Average overall length of queue: 0.113718




Maximum length of primary queue: 1

Maximum length of secondary queue: 3

Average maximum length of queue: 2

Maximum length of overall queue: 4




Total idle time for each server:

Primary server 0: 128 minutes

Primary server 1: 98 minutes

Primary server 2: 98 minutes

Primary server 3: 107 minutes

Primary server 4: 115 minutes

Primary server 5: 96 minutes




Secondary server 0: 146 minutes

Secondary server 1: 143 minutes

Secondary server 2: 123 minutes

Secondary server 3: 110 minutes

Secondary server 4: 137 minutes

Secondary server 5: 133 minutes




Simulation ends after 277 minute(s) or 4.61667 hour(s) of simulation process. Simulation End Time: Sat Jul 24 02:18:51 2021




YCT-MacBook:csci203 sionggojapit$







<strong>Standard Requirements for Part B (Programming question): </strong>

<strong> </strong>

<ul>

 <li>Java Version – JDK 6 update 17 or higher (Using Windows), or</li>

 <li>C++ / C compiler – g++ 4.0 or higher (Using Windows or UBUNTU). In the event that you use UBUNTU via VM, be careful with the memory function of the language and make sure that the functions are used properly and do not cause any segmentation error when the codes are compiled in Windows environment.</li>

 <li>All coding must be your own work. Standard libraries of data structures and algorithms such as STL may not be used.</li>

 <li>Programs should be appropriately documented with comments.</li>

 <li>Execute your program and screen-capture the output. Include in your submission all source code and libraries plus the screen-captures.</li>

 <li>Students are to place all compilation and instructions on how to run the program inside a readme.txt file. Your lecturer will refer to this file when marking. Without a readme.txt or clear instructions for compilation, your lecturer will compile based on his/her computer setting; any incompatibility, will deem as failure to compile the program.</li>

 <li>Submission filenames are to follow the naming convention given in the submission instruction below. Do not use your own filename.</li>

</ul>




<ul>

 <li>For Part A, type your answer for each question in a MS Word or equivalent document format and save it in a pdf formatted file, name your file as YourUOWStudentNumber-A2-SolPartA.pdf.</li>

 <li>For Part B, the name of your program should be QueueSim.cpp or QueueSim.java, depending on the programming language that you use to develop your program. Execute your program and <strong>screen capture</strong> your output. Next, zip your source code, libraries, readme.txt together with your screen capture and name your file as YourUOWStudentNumber-A2-SolPartB.zip.</li>

 <li>Zip together YourUOWStudentNumber-A2-SolPartA.pdf and YourUOWStudentNumber-A2-SolPartB.zip and name your file as</li>

</ul>

YourUOWStudentNumber-A2.zip. Do not use your own filename.

<ul>

 <li>All assignments that do not satisfy the submission requirements listed above will not be evaluated and will be returned to the students with 0 marks.</li>

</ul>