# Spring Boot Project

Please finish and submit the following project in the required time.

Description:
One professor would like to use a web application to create new courses.
Professor will create several courses for a few students, and students can select courses.

Backend APIs required to fulfill:  

For Professor: APIs that can create courses
1.	can create each course. (postMapping --> input: name, description text; output: Course)
2.	can delete each course. (postMapping --> input: course id; output: status message indicating delete success or failure)
4.	can edit description text on each course. (postMapping --> input: course id, course description; output: status message indicating success or failure)
5.	can update roster of attended students if they join or quit course.
6.	can check how many students select each course and who they are (name and gender). 
7.	can check anonymous text reviews from students on each course and send back text message to any reviews.
8.	can check anonymous numerical ratings (0-10 inclusive) from students on each course.
9.	can check highest rating, lowest rating, and the average rating score.
10.	can sort the text reviews in ascending and descending order according to updated time of reviews.
11.	can get the review text containing String keyword “good” and “bad”.

For Students: APIs that check and select courses
1.	can read texts that describes each course.
2.	can join any courses. (postMapping --> input: student id, course id) 
3.	can quit any courses. (postMapping --> )
4.	can write text reviews to any courses that he attended before.
5.	can send numerical rating to any course that he attended before.

![Diagram](https://user-images.githubusercontent.com/112025981/188248437-efc8a985-6144-4fcb-a3fa-c570f3081f82.svg)

Project Requirements:
1.	Generate a Gradle or Maven Project with Java and Spring Boot framework (version 2.7.3).
  1.1 Group name: com.vibrant  
  1.2 Artifact name: demo  
2.	Database: use H2 in-memory database  
  2.1 Store the database entity for use
3.	Configure your Spring Boot project so that the project can be run.
4.	It is a plus if you configure swagger in project package.  
  4.1 SpringFoxConfig → configure swagger for API testing (refer to picture below as an example:   http://localhost:Your Port Number/swagger-ui/#/)
  ![Picture1](https://user-images.githubusercontent.com/112025981/188246311-e6abaa18-153e-4f18-ad40-e8b182555a23.svg)
5.	Use Spring Data JPA dependency to implement JPA for database manipulations 
6.	In your project, please pick at least one API to implement the Junit test. It is required to have 3 test cases for the according API which can demonstrate the developed API passes all 3 test cases.
