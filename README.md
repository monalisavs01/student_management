University Student Database


This project designs and implements a relational database for a student database system to track student details.

The database schema consists of the following tables:

user_login: Stores user login information such as user ID, password, name, signup date, and email.

parent_details: Stores details about parents, including parent ID, names, email, mobile numbers, and occupations.

teachers: Stores information about teachers, including teacher ID, names, date of birth, email, contact details, registration date, and registration ID.

class_details: Stores information about classes, including class ID, class teacher (reference to teacher), and class year.

student_details: Stores details about students, including student ID, names, date of birth, class ID (reference to class_details), roll number, email, parent ID (reference to parent_details), registration date, and registration ID.

subject: Stores information about subjects, including subject ID, subject name, class year, and subject head (reference to teacher).

subject_tutors: Acts as a junction table to assign teachers as tutors for specific subjects in specific classes. It includes a row ID (auto-incrementing), subject ID (reference to subject), teacher ID (reference to teacher), and class ID (reference to class_details).
