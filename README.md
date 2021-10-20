# University Student Dimensional Model
Examined Northeastern University's graduate student course enrollment and performance for two MS programs: 
1. Information Systems 
2. Data Architecture and Management

The project went through three phases of data model design:

I) Requirements: Gather, analyse and prioritize business requirement
Business:
1. What are the core requirements and elective courses for these programs
2. What classes (course & section) did students complete in a semester & what were their grades?
3. What were the enrollment and drop dates if applicable for students in each class in a semester?
4. Who were the teachers in each class above?
5. What were the classes taught each semester?
6. What teachers taught classes in a degree program in a semester?
7. Who are the students enrolled in a degree program and attributes such as ID, email, date of birth (DOB), hometown, campus/off-campus address if applicable, etc?

Data:
Identified high level entities and measures (metrics)
1. College, Department
2. Degree Programs
3. Semesters
4. Courses
5. Classes (course, section, semester)
6. Students
7. Teachers
8. Course grades

II) Logical Data Model

Identified Facts & Grain
1. Identified grain(s) in business processes 
2. Identified Fact Tables
3. Identified Fact Table Types
  3.1 Transaction
  3.2 Periodic
  3.3 Accumulating
4. Identified Fact Table Granularity
5. Identified preliminary dimensions

Determined dimensions:
1. Identified degenerate & conformed dimensions
2. Identified dimensional attributes & validate granularity
3. Identified hierarchies & attributes
4. Identified date & time attributes
5. Identified slowly changing dimensions (SCD) & types
6. Identified multi-valued dimensions & define approach
7. Identified role-playing dimensions
8. Identified & classify specialized dimensions
  8.1. Junk, Rapidly Changing, Hot Swappable, etc
9. Define surrogate keys (SKs), identify natural keys (NKs) and alternative keys (AKs)
10. Define change data capture (CDC) attributes

Determined facts:
1. Identified conformed facts
2. Identified fact attribute types
  2.1 Additive
  2.2 Semi-additive
  2.3 Non-additive
3. Identify derived attributes & define approach
4. Identify aggregates with associated hierarchies & define approach
5. Identify composite keys & design PK approach
6. Identify “snapshot” tables & define approach
7. Identify event tables & define approach


III) Physical Data Model
1. Created dimensional data model using ER Studio. 
2. Created SQL DDL (data definition language) scripts to create tables and columns with primary keys (PKs) and foreign keys (FKs) defined.
3. Created sample data using faker() class in python, stored in a .csv file
4. Loaded sample data using Alteryx
5. Visualizations on a PowerBI dashboard




