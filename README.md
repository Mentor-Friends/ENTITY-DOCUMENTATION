# ENTITY-DOCUMENTATION

# ENTITY

A brief description of ENTITY.

An entity can refer to any identifiable object or thing that exists. It could be a person, place, thing, or concept. The term is often used in a broad, abstract sense to describe any discrete and separately identifiable unit.

In the context of databases and data modeling, an entity refers to a distinct object, concept, or thing about which data can be stored. It is often represented as a table in a relational database. Each row in the table represents an instance of that entity, and each column represents an attribute or property of the entity.
![Entity ](https://github.com/Mentor-Friends/ENTITY-DOCUMENTATION/assets/155048883/e8bf21cb-a9ae-4142-ac4d-ac20aefa566e)


# TYPES OF ENTITY.

**Physical Entity:** Referring to tangible objects like a car or a book.

**Abstract Entity:** Referring to conceptual entities like a project or a process.





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

