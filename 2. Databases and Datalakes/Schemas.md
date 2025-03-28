[L5DE M2T2 v1.pdf](https://github.com/user-attachments/files/19410510/L5DE.M2T2.v1.pdf)

The relational model is a foundational framework in database management, introduced by E.F. Codd in 1970. It organizes data into tables (relations) consisting of rows (tuples) and columns (attributes), ensuring data integrity and reducing redundancy.

Key Terminology:
Relation (Table):

A set of data organized into rows and columns.

Represents an entity or a concept (e.g., "Students" table).

Tuple (Row/Record):

A single entry in a table.

Represents one instance of an entity (e.g., one student’s details).

Attribute (Column/Field):

A characteristic or property of the entity.

Defines the type of data stored (e.g., "Student_Name").

Domain:

The allowable set of values for an attribute (e.g., age must be a number).

Primary Key:

A unique identifier for each tuple in a table (e.g., "Student_ID").

Foreign Key:

An attribute in one table that refers to the primary key of another table.

Establishes relationships between tables (e.g., "Course_ID" in a "Student" table linking to a "Courses" table).

Candidate Key:

A set of attributes that uniquely identify a tuple.

One candidate key is chosen as the primary key.

Super Key:

A set of attributes that uniquely identifies a tuple but may contain additional unnecessary attributes.

Composite Key:

A primary key that consists of multiple attributes (e.g., "Order_ID" + "Product_ID" in an order system).

Normalization:

The process of organizing data to eliminate redundancy and dependency issues.

Achieved through normal forms (1NF, 2NF, 3NF, BCNF, etc.).

Integrity Constraints:

Entity Integrity: Primary keys must have unique values and cannot be NULL.

Referential Integrity: Foreign keys must reference valid primary key values in another table.

Relational Algebra:

A set of operations (Selection, Projection, Join, Union, etc.) used to manipulate relational data.
