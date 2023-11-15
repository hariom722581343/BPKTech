# BPKTech
Index.html  file is main file.




SQL


Since the job requires excellent database knowledge and algorithm skill, please complete the following task.
• For a school, I would like to store the marks for all the students of grade 1 to 8 for all the subjects they study.
o Design a table structure to store the student marks in all subjects.
CREATE TABLE student_marks (
  student_id INT PRIMARY KEY NOT NULL,
  subject VARCHAR(255) NOT NULL,
  marks INT NOT NULL,
  grade INT NOT NULL
);
o Design a screen to add new student details (f.name, l.name, dob, parent's name, address, city, phone#) and show the list of students with this data in a table as and when it is created.
Create a table to store student details:->
CREATE TABLE students (student_id INT PRIMARY KEY,
first_name VARCHAR(50) NOT NULL,
last_name VARCHAR(50) NOT NULL,
dob DATE NOT NULL,
parent_name VARCHAR(100) NOT NULL,
address VARCHAR(255) NOT NULL,
city VARCHAR(50) NOT NULL,
phone_number VARCHAR(20) NOT NULL,
subject VARCHAR(50) NOT NULL,
marks INT NOT NULL,
grade VARCHAR(5) NOT NULL);
display the list of students:->
SELECT * FROM students;




o Generate a report that will show all the students who have scored more than 60%.
SELECT student_id, first_name, last_name, subject, marks, grade
FROM student_marks
WHERE marks > 60;
