# Spring Boot Project

Please finish and submit the following project in the required time.

Description:
One professor would like to use a web application to create new courses.
Professor will create several courses for a few students, and students can select courses.

Backend APIs required to fulfill:
For Professor: APIs that can create courses
1.	can create and edit text to describe each course.
2.	can update roster of attended students if they join or quit course
3.	can check how many students select each course and who they are (name and gender). 
4.	can check anonymous text reviews from students on each course and send back text message to any reviews.
5.	can check anonymous numerical ratings (0-10 inclusive) from students on each course.
6.	can check highest rating, lowest rating, and the average rating score.
7.	can sort the text reviews in ascending and descending order according to updated time of reviews.
8.	can get the review text containing String keyword “good” and “bad”.

For Students: APIs that check and select courses
1.	can read texts that describes each course.
2.	can select or quit any courses.
3.	can write text reviews to any courses that he attended before.
4.	can send numerical rating to any course that he attended before.

![Diagram](https://user-images.githubusercontent.com/112025981/188245719-739ae91f-bb76-406e-ad9d-861c58bc7b1f.svg)

Project Requirements:
1.	Generate a Gradle or Maven Project with Java and Spring Boot framework (version 2.7.3).
  1.1 Group name: com.vibrant
  1.2 Artifact name: demo
2.	Database: use H2 in-memory database
  2.1 Store the database entity for use
3.	Configure your Spring Boot project so that the project can be run.
4.	It is a plus if you configure swagger in project package.
  4.1 SpringFoxConfig → configure swagger for API testing (refer to picture below as an example:   http://localhost:Your Port Number/swagger-ui/#/)
5.	Use Spring Data JPA dependency to implement JPA for database manipulations 
6.	In your project, please pick at least one API to implement the Junit test. It is required to have 3 test cases for the according API which can demonstrate the developed API passes all 3 test cases.
