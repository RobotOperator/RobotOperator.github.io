# Robot Operator's Github Portfolio
A collection of Lance Cain's (aka. Robot Operator) software development and Computer Science work hosted by Github Pages.

* TOC
{:toc}

## My Work in Computer Science at SNHU

This portfolio contains projects that I developed and enhanced during my academic journey at Southern New Hampshire University (SNHU). As the final part of my learning program I chose to enhance the below included projects as a demonstration of my ability to:

  1. Employ strategies for building collaborative environments that enable diverse audiences to support organizational decision making in the field of computer science
  2. Design, develop, and deliver professional-quality oral, written, and visual communications that are coherent, technically sound, and appropriately adapted to specific audiences and contexts 
  3. Design and evaluate computing solutions that solve a given problem using algorithmic principles and computer science practices and standards appropriate to its solution, while managing the trade-offs involved in design choices (data structures and algorithms) 
  4. Demonstrate an ability to use well-founded and innovative techniques, skills, and tools in computing practices for the purpose of implementing computer solutions that deliver value and accomplish industry-specific goals (software engineering/design/database) 
  5. Develop a security mindset that anticipates adversarial exploits in software architecture and designs to expose potential vulnerabilities, mitigate design flaws, and ensure privacy and enhanced security of data and resources
  
This portfolio demonstrates a great many skills that I gained through my studies as SNHU through publicly shared projects incorporating Python, PHP, Java, MongoDB, and SQLite. If you have an interest in learning a bit more about my development capabilities please feel free to reach out to me directly about some of my private projects featuring C#, Python, PowerShell, Bash, C++, and more. 
 
## 1. Professional Assessment 
Pending.

## 2. Code Review
The enhancements I performed as part of my final project in CS499 started with a code review of the existing software projects I previously created.
The code review serves as a demonstration of my capabilities to create a presentation combining oral and visual media delivering accurate technical concpets in a coherent, easy to understand manner, that is tailored to my audience. The review is presented in an informal manner that covers the previous state of each of the artifact submissions I have included below.

The original full-scale video hosted on YouTube can be viewed [here](https://youtu.be/0v01YbG2tHA).
<iframe src="https://youtube.com/embed/0v01YbG2tHA" width="420" height="315"></iframe>

## 3. [Grazioso Dashboard](https://github.com/RobotOperator/GraziosoDashboardEnhanced) - Software Design and Engineering
I have chosen to improve the Grazioso Dashboard that I created in CS340 Client Server Development at SNHU. This dashboard was developed as a full stack project with a MongoDB backend, Python middleware module that performed CRUD actions with database, and a Jupyter Notebook web front end that presented animal records to users as well as a graph and map relating to records presented. The initial version of this project is available in my code repositories [here](https://github.com/RobotOperator/CS340-GraziosoDashboard). This project presents a great example of my abilities to create full-stack software solutions with intuitive an UI that demonstrates an ability to use well-founded and innovative techniques, skills, and tools in computing practices for the purpose of implementing computer solutions that deliver value and accomplish industry-specific goals. 

I chose to to improve this project by re-implementing the client front-end and middleware functionality for interacting with the database in PHP as well as adding required user authentication to access the data in the dashboard. Re-implementing this project in PHP makes it far more versatile for deployment across a wide range of well supported webservers like Apache, NGinx, and IIS. Throughout the process of enhancing this project I learned a great deal of new information pertaining to PHP function calls, AJAX JQL queries, and authenticated session tracking for web servers. Many of the cleint side rendered functionality of this project that was previously handled by Python Dash modules were not avaialbe when working in PHP. This offered me the opportunity to both learn more about client side web technologies like javascript and more accurately control the client side content rendered for the dashboard of this project. As a result, I was able to make the interactions with Dashboard for searching and filtering a bit more intuitive with a dedicated search bar as well as gain experience using an established technique of using AJAX queries for populating dynamic content in HTML fields. 

One of the motivations for my multiple improvements to this project was a desire to improve the security of the dashboard with the addition of a required login screen as well as individual session tracking for accessing data in the MongoDB backend. The orginal application used a statically configured service account to access records in the database without any prior authentication from clients. The improvements I developed now resolve the need for including any static embedded credentials in the code as well as place more control in the hands of applicaiton administrators to create users in the MongoDB server prior to them being able to access the stored data.

Some of the greatest challenges I overcame when working on these enhancements was working in depth with dynamic client-side rendered web content. I understand now why my college had us create the original project with Python flask and dash since those modules handled many complex aspects of the dashboard like creating the graph and map widgets with little required configuraiton. I was able to replicate all of the previous functionality in PHP with rendered HTML content using some supporting javascript and a fair amount of research.

## 4. [Contact Service](https://github.com/RobotOperator/ContactService) - Data Structure and Algorithms
The second project I chose to improve as part of my final project in CS499 is a Contact Service application I developed using Java for my CS320 Testing, Automation, and Quality Assurance course at SNHU, original project available [here](https://github.com/RobotOperator/CS320-ContactService). The ContactService and Contact java classes were developed according to a client’s need to be drop in objects for larger programs to store user contact information. I developed two Junit5 classes, ContactServiceTest and ContactTest, to serve as unit tests for these classes that used both positive testing and negative testing to validate the classes would only accept data that met the customer’s specifications for length and type. This artifact was my first exposure to unit testing and helped me gain an understanding of how beneficial proper testing could be when determining not only expected logic execution flows but also error handling for deviations from the expected flow. 

I chose to include this artifact in my portfolio because it demonstrates proficiency in creating unit tested software and awareness of making use of efficient searching when indexing all of the Contacts in the service using their id attributes. I chose to enhance this artifact in two primary ways by first adding a Driver class to serve as a user interface for interacting with the application and second by adding SQLite database storage to serve as persistent storage for the application. The enhancements I added within the Driver class created a new class that validates user supplied data, implements error handling for both specific and general exceptions, uses multiple logic structures such as while and if statements to branch execution making it more efficient, and relies on calls to internal methods implementing both abstraction and simplified logic execution using separate functions. I also improved the Contact and ContactService classes by adding explicit information to the InvalidArgument errors thrown by these classes which now include the offending statements/supplied arguments to help both users and developers remedy the issue. During the development process I learned that the Contact and ContactService classes I had originally created were not as intuitive to use for development handling errors which I corrected by sanitizing and casting input to lower case for some of the method calls that rely on string comparisons.

Enhancing this project to be a stand-alone Java application using a command-line interface with the ability to create retrieve, update, and delete contact information stored within the service based on validated user input serves as a demonstration of my proficiency in working with algorithms and data structures. The final project resulted in the creation of additional methods, attributes, as well as two dbConnector and dataEncrypt classes that facilitate integration with the second primary enhancement of creating a persistent storage using a local SQLite database. I created additional unit tests for the database connections and encryption that I developed during my enhancements of this project which continued the practice of positive and negative testing the newly created class functiolity to ensure errors were thrown and handled as expected. The validation and testing performed for proper error handling within the classes of this project also demonstrates designing and developing code early on with a security mindset with the intent to prevent adversarial exploit of the appication through any vulnerabilities, mitigate design flaws, and ensure enhanced security and enhanced security of resources.

One of the biggest challenges I encountered during this enhancement was properly delimiting and interpreting user supplied input to be validated against the underlying classes from standard input. After some time of checking for and working with user supplied input that contained whitespace in supplied strings I ended up creating checks for whole line inputs on Windows using the standard '\r\n' carriage return input at certain decision points in the new Driver class which addressed the problems I was encountering. The user input interface has now been refined with some minor additions to handle any supplied input to include malformed datasets and safely handle those cases. I also found myself continuously working to keep the existing unit tests I had previously developed updated as I continued to improve upon and expand the existing classes to fulfill new functionality in the application. I ensured that any new additions I created to the code was both fully tested and did not break any prior existing functionality by testing frequently locally.

## 5. [Contact Service](https://github.com/RobotOperator/ContactService) - Database Proficiency
The Contact Service application also serves as a demonstration of my proficiency in designing and integrating databases in software development. When I created the two classes for this project with the associated unit tests they were designed to run solely in memory using Java ArrayLists. I improved upon this by integrating a local SQLite database for the application to serve as a persistent storage ensuring that data would not be lost whenever the service was interrupted or required shutdown. My thoughts behind this enhancement was that it would make the Java application more flexible to be used by many different individuals across different platforms rather than requiring 100% consistent uptime while the service was running making the code adaptable to a more diverse group of individuals that are working and making decisions in the field of Computer Science.   

The Contact Service application now automatically checks for the database existence and connectivity prior to proceeding with any execution and appropriately handles any errors to recreate the database locally if needed, which demonstrates some of my additional experience in working with Data Structures and Algorithms. Enhancing the application using SQLite was a great learning experience expanding my understanding of working with prepared statements to safely perform queries against the underlying database to create, retrieve, update, and delete contact records. The choice to implement my own dbConnector class that was then called and instantiated within the Contact Service class meant that the queries being performed against the underlying database were benefitting from the input validation I had previously implemented in that service. I chose to implement the database with XOR encryption for stored data using a key supplied upon application startup to protect contact information stored within it to prevent any offline viewing or retrieval for early security. I chose to make the database connection class flexible and adaptable to multiple types of SQL databases by using the built in Java SQL libraries with an sqlite-jdbc driver for interacting with the SQLite storage which could be replaced with almost any other jdbc driver to facilitate connecting to other databases across a network. 

When choosing to include a database in the Contact Service application I began balancing the positives and negatives of the technology for underlying storage. Despite some additional latency introduced to the application when inserting and updating contacts I believe I made the right decision since the application now automatically loads prior contacts on startup rather than requiring users to resubmit them if the service is restarted. I was able to mitigate some of the trade-offs by continuing to use in memory ArrayLists when retrieving and searching for contacts that quickly returns desired data without needing to query the database. This enhancement demonstrates my abilities to consider computing solutions that solve a given problem using algorithmic principles and computer science practices and standards appropriate to its solution, while managing the trade-offs involved in design choices.

## 6. Other Academic Work
[CS 405](https://github.com/RobotOperator/CS405) - Secure Coding C++ work
<br>[CS 330](https://github.com/RobotOperator/CS330) - OpenGL 3D Design 
<br>[CS 250](https://github.com/RobotOperator/CS250) - Agile Team Development Restrospective
