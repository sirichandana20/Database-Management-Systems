Please create the ER Diagram for eLearn based on the following description.


eLearn is an e-learning platform. Learners can explore, enroll, study and get certificates from a variety of courses. Courses are grouped into multiple categories. A course may be presented in different categories. Each course has a unique course id (a number with two prefix letters – for example, CS585) and consists of materials, lectures and assignments. 
Materials could be general (for example, syllabus, textbook) or come from a lecture. Each lecture may have videos, notes, and materials (files, links...). Each assignment has a description, attached files and a deadline. Learners must submit their assignments online. Learners can view their grades for each assignment (quite similar to USC blackboard). 
With lectures and assignments, learners and teacher may post comments. This is useful for teacher to provide any additional notes about the questions being asked, or for students to ask any questions regarding the lectures or assignments. 
A user has to register to enroll a course. Prices may vary from different courses. Different payment methods are available (e.g. Visa/Master Card, Paypal, Bitcoin). The handling of payment details could be outside of eLearn for security reasons. The system should be flexible enough to easily add new payment method or remove an existing one. 
After completing the course, a user can see his/her grades in details and gets a certificate (if eligible). He/she can also rate the course (0-5 stars) or provide feedback. 
A course is created by its teacher. Multiple teachers are allowed to get involved in a course. There are also other roles (TA, graders) who have different permissions on different course operations. 
A course should start and end at certain time. It can be re-opened multiple times, for example, per semester or per year. Each time it is re-opened, there may be multiple adjustments (teachers, TA and graders, students, course content, assignments).
Feel free to make additional assumptions if they are not stated in the description (for example, attributes of entities). You also should be able to analyze the trade-offs of your design decisions.
