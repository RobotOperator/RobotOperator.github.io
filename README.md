# Robot Operator's Github Portfolio
A collection of Lance Cain's (aka. Robot Operator) software development and Computer Science work hosted by Github Pages.

* TOC
{:toc}

## My Work in Computer Science at SNHU

This portfolio contains projects that I developed and enhanced during my academic journey at Southern New Hampshire University (SNHU). As the final part of my learning program I chose to enahnce the below included projects as a demonstration of my ability to:

  1. Employ strategies for building collaborative environments that enable diverse audiences to support organizational decision making in the field of computer science
  2. Design, develop, and deliver professional-quality oral, written, and visual communications that are coherent, technically sound, and appropriately adapted to specific audiences and contexts 
  3. Design and evaluate computing solutions that solve a given problem using algorithmic principles and computer science practices and standards appropriate to its solution, while managing the trade-offs involved in design choices (data structures and algorithms) 
  4. Demonstrate an ability to use well-founded and innovative techniques, skills, and tools in computing practices for the purpose of implementing computer solutions that deliver value and accomplish industry-specific goals (software engineering/design/database) 
  5. Develop a security mindset that anticipates adversarial exploits in software architecture and designs to expose potential vulnerabilities, mitigate design flaws, and ensure privacy and enhanced security of data and resources
  
This portfolio demonstrates a great many skills that I gained through my studies as SNHU through publicly shared projects incorporating Python, PHP, Java, MongoDB, and SQLite. If you have an interest in learning a bit more about my development capabilities please feel free to reach out to me directly about some of my private projects featuring C#, Python, PowerShell, Bash, C++, and more. 
 
## 1. Professional Assessment 
Pending.

## 2. Code Review
The enhancements I performed as part of my final project in CS499 started with a code review of the existing software projects I created that can be found [here](https://youtu.be/0v01YbG2tHA).
The code review serves as a demonstration of my capabilities to create a presentation combining oral and visual media delivering accurate technical concpets in a coherent, easy to understand manner, that is tailored to my audience.

## 3. [Grazioso Dashboard](https://github.com/RobotOperator/GraziosoDashboardEnhanced)
I have chosen to improve the Grazioso Dashboard that I created in CS340 Client Server Development at SNHU. This dashboard was developed as a full stack project with a MongoDB backend, Python middleware module that performed CRUD actions with database, and a Jupyter Notebook web front end that presented animal records to users as well as a graph and map relating to records presented. The initial version of this project is available in my code repositories [here](https://github.com/RobotOperator/CS340-GraziosoDashboard). This project presents a great example of my abilities to create full-stack software solutions with intuitive UIs.

I chose to to improve this project by re-implementing the client front-end and middleware functionality for interacting with the database in PHP as well as adding required user authentication to access the data in the dashboard. Re-implementing this project in PHP makes it far more versatile for deployment across a wide range of well supported webservers like Apache, NGinx, and IIS. Throughout the process of enhancing this project I learned a great deal of new information pertaining to PHP function calls, AJAX JQL queries, and authenticated session tracking for web servers. Many of the cleint side rendered functionality of this project that was previously handled by Python Dash modules were not avaialbe when working in PHP. This offered me the opportunity to both learn more about client side web technologies like javascript and more accurately control the client side content rendered for the dashboard of this project. As a result, I was able to make the interactions with Dashboard for searching and filtering a bit more intuitive with a dedicated search bar as well as gain experience using an established technique of using AJAX queries for populating dynamic content in HTML fields. 

One of the motivations for my multiple improvements to this project was a desire to improve the security of the dashboard with the addition of a required login screen as well as individual session tracking for accessing data in the MongoDB backend. The orginal application used a statically configured service account to access records in the database without any prior authentication from clients. The improvements I developed now resolve the need for including any static embedded credentials in the code as well as place more control in the hands of applicaiton administrators to create users in the MongoDB server prior to them being able to access the stored data.

Some of the greatest challenges I overcame when working on these enhancements was working in depth with dynamic client-side rendered web content. I understand now why my college had us create the original project with Python flask and dash since those modules handled many complex aspects of the dashboard like creating the graph and map widgets with little required configuraiton. I was able to replicate all of the previous functionality in PHP with rendered HTML content using some supporting javascript and a fair amount of research.


## 4. Contact Service - Part 1
Pending.

## 5. Contact Service - Part 2
