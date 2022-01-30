CREATE DATABASE students;
CREATE TABLE student(
	studentId int PRIMARY KEY IDENTITY(1,1),
	studentName varchar(30),
	lessonName varchar(30),
	examPoint int,
	situation varchar(10)
);
INSERT INTO student(studentName, lessonName, examPoint, situation) VALUES ('Leonard', 'German', 35, 'fail'), 
('Sue', 'English', 60, 'pass'), ('Richard', 'Geography', 90, 'pass'), ('Ashley', 'Physics', 12, 'fail'),
('Sam', 'German', 72, 'pass'), ('William', 'German', 22, 'fail'), 
('Julliet', 'Physics', 60, 'pass'), ('Richard', 'Geography', 68, 'pass'), ('Will', 'English', 96, 'pass'), 
('Allen', 'Physics', 22, 'fail'), ('Sort', 'Physics', 52, 'fail'), ('Cortney', 'English', 40, 'fail'), 
('Jack', 'Physics', 41, 'fail'), ('Park', 'Geography', 70, 'pass'), ('Zoe', 'Physics', 46, 'fail'), 
('Allen', 'Physics', 60, 'pass');

SELECT * FROM student;
SELECT DISTINCT studentName FROM student;
SELECT COUNT(DISTINCT studentName) FROM student;
SELECT studentName, lessonName, examPoint FROM student WHERE situation='pass'; 
SELECT studentName, examPoint FROM student WHERE examPoint>30; 
UPDATE student SET examPoint=12 WHERE (examPoint=22 AND studentName='Allen');
SELECT * FROM student ORDER BY examPoint DESC;
SELECT AVG(examPoint) FROM student;
SELECT studentId, studentName, lessonName, examPoint FROM student WHERE examPoint > (SELECT AVG(examPoint) FROM student);
