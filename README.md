# ENTITY-DOCUMENTATION

# ENTITY

A brief description of ENTITY.

An entity is a distinguishable and meaningful object or concept that can be identified and described. Examples of entities include customers, products, employees, and orders.

An entity can refer to any identifiable object or thing that exists. It could be a person, place, thing, or concept. The term is often used in a broad, abstract sense to describe any discrete and separately identifiable unit.

In the context of databases and data modeling, an entity refers to a distinct object, concept, or thing about which data can be stored. It is often represented as a table in a relational database. Each row in the table represents an instance of that entity, and each column represents an attribute or property of the entity.

**Attributes:**

Each entity has attributes that describe its properties. For example, a "Customer" entity might have attributes such as "CustomerID," "FirstName," "LastName," and "Email."

**Entity-Relationship Diagram (ERD):**

ERD is a graphical representation that illustrates the relationships between entities. Entities are represented as rectangles, and relationships are depicted by connecting lines.

1. An Entity-relationship Diagram (ER Diagram) describes the relationship of entities that need to be stored in a database. 

2. ER Diagram is mainly a structural design for the database. It is a framework using specialized symbols to define the relationship between entities.  

3. ER diagram is created based on three main components entities, attributes, and relationships.

      ![ERD](https://github.com/Mentor-Friends/ENTITY-DOCUMENTATION/assets/155048883/ededb8af-ccc9-4dc9-af4d-4347497200c5)

       The above diagram show case in two entities student and course and the relationship. The relationship describe between student and course is many to many. As a course can be octed by several student . As  a student can more than one course. Here student is the entities  and it’s possessive attributes that is student id , student name, and student age. And the course attributes such as course id, and course name . 

**TYPES OF ENTITY.**

**Physical Entity:** Referring to tangible objects like a car or a book.

**Abstract Entity:** Referring to conceptual entities like a project or a process.


**Primary Key:**

An entity typically has a primary key, which is a unique identifier for each instance of the entity. This key is used to distinguish one entity instance from another.

**Relationships:**

Entities can be related to each other through relationships. Common relationship types include one-to-one, one-to-many, and many-to-many. These relationships help define how data is connected and organized in the database.

## Example Entity in an ERD:

Consider a simplified e-commerce scenario:

**Entity: Customer**
Attributes: CustomerID (Primary Key), FirstName, LastName, Email
Relationships: May be related to the "Order" entity through a one-to-many relationship (a customer can place multiple orders).

## Basic Steps for Modeling Entities in a Database:

1. Identify Entities:

Recognize the main objects or concepts relevant to your application.

2. Define Attributes:

Identify and define the properties (attributes) that describe each entity.

3. Establish Relationships:

Determine how entities are related to each other. Use relationships to connect entities and define the cardinality (e.g., one-to-many).

4. Assign Primary Keys:

Choose or create a unique identifier (primary key) for each entity.

5. Create an Entity-Relationship Diagram (ERD):

Use an ERD to visually represent entities, attributes, and relationships.
Remember that the specifics can vary depending on the database management system (DBMS) you are using (e.g., MySQL, PostgreSQL, Microsoft SQL Server). Documentation for your specific DBMS may provide additional details and best practices for entity modeling.


## Usage/Examples

 A "person entity with connection type, Let's consider a simple example with a "Person" entity and a "Connection" entity to represent relationships between people:

**Person Entity:**

***Attributes:***

**PersonID (Primary Key):** A unique identifier for each person.

**FirstName:** The first name of the person.

**LastName:** The last name or surname of the person.

**DateOfBirth:** The date of birth of the person.

**Address:** The current address of the person.

**Email:** The email address of the person.

**PhoneNumber:** The phone number of the person.


**Connection Entity:**

***Attributes:***

***ConnectionID (Primary Key):*** A unique identifier for each connection.

**Person1ID (Foreign Key):** The PersonID of the first person in the connection.

**Person2ID (Foreign Key):** The PersonID of the second person in the connection.

**RelationType:** The type of relationship or connection between the two persons (e.g., "Friend," "Family," "Colleague").

In this model, the "Connection" entity represents relationships between individuals. The "Person1ID" and "Person2ID" are foreign keys that reference the "PersonID" in the "Person" entity, creating a connection between two individuals. The "RelationType" attribute describes the type of relationship.

Here's a simplified representation:

***Person Table:***

| PersonID | FirstName | LastName | DateOfBirth | Address  | Email                          | PhoneNumber |
| -------- | :-------- | -------- | ----------- | -------- | ------------------------------ | ----------- |
| 1        | Santosh   | Yadav    | 1993-08-25  | Janakpur | santoshyadav@Mentorfriends.com | 9860709636  |
| 2        | Bhanu     | Singh    | 1990-08-22  | Siraha   | bhanusingh@mentorfriends.com   | 9818097288  |

***Connection Table:***

| ConnectionID | Person1ID | Person2ID | RelationType |
| ------------ | --------- | --------- | ------------ |
| 101          | 1         | 2         | Friend       |
| 102          | 1         | 3         | Colleague    |

In this example, the "Connection" table establishes connections between persons. Connection 101 indicates that Person 1 (Santosh) is a friend of Person 2 (Bhanu), and Connection 102 indicates a colleague relationship between Person 1 and another person with ID 3.

