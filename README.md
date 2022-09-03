# Spring Boot Project

Please finish and submit the following project in the required time.

Description:
One professor would like to use a web application to create new courses.
Professor will create several courses for a few students, and students can select courses.

Backend APIs required to fulfill:  

For Professor: APIs that can create courses  
1.can create each course. (postMapping course table --> input: name, description text, active status; output: Course)  
2.can delete each course. (postMapping course table --> input: course id, active status; output: status message indicating delete success or failure    	                                          update Enrollment table --> input: course id, false; output: status message indicating delete success or failure)
3.can edit description text on each course. (check course table --> input: course id; ouput: course active status  
	                                    postMapping course table --> input: course id, course description; output: status message indicating success or failure)  
4.can remove student from course. (postMapping enrollment table --> input: course id, student id, false; output: status message indicating success or failure)  
5.can check how many students select each course. (check course table --> input: course id; ouput: course active status  
                                                   getMapping course table --> input: course id; output: number of List<Student>)   
6.can check enrolled students'information. (check course table --> input: course id; ouput: course active status  
                                            getMapping course table --> input: course id; output: List<Student>)     

For Students: APIs that check and select courses  
1.can read texts that describes on each course. (check course table --> input: course id; ouput: course active status  
                                                 getMapping course --> input: course id; output: course description)  
2.can join any courses. (check course table --> input: course id; ouput: course active status  
                         postMapping enrollment table --> input: student id, course id, true; output: status message indicating success or failure)   
3.can quit any courses. (postMapping enrollment table --> input: student id, course id, enrolled status true; output: status message indicating success or failure)  

![Diagram](https://user-images.githubusercontent.com/112025981/188248437-efc8a985-6144-4fcb-a3fa-c570f3081f82.svg)

Project Requirements:
1.Generate a Gradle or Maven Project with Java and Spring Boot framework (version 2.7.3).
  1.1 Group name: com.vibrant  
  1.2 Artifact name: demo  
2.Database: use H2 in-memory database  
  2.1 Store the database entity for use
3.Configure your Spring Boot project so that the project can be run.
4.It is a plus if you configure swagger in project package.    
  4.1 SpringFoxConfig → configure swagger for API testing (refer to picture below as an example:   http://localhost:Your Port Number/swagger-ui/#/)  
  ![Picture1](https://user-images.githubusercontent.com/112025981/188246311-e6abaa18-153e-4f18-ad40-e8b182555a23.svg)
5.Use Spring Data JPA dependency to implement JPA for database manipulations 
6.In your project, please pick at least one API to implement the Junit test. It is required to have 3 test cases for the according API which can demonstrate the developed API passes all 3 test cases.
