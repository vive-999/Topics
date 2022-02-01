###	<center>		**Entity Relationship Diagram(ERD)** </center>
  
**_ER-Diagram is a pictorial representation of data that describes how data is communicated and related to each other._**
In other words, Entitiy Relationship is the Connection between  fields(colums) of an entity(table) to anther field of another entity or same entity so that the two entities can be related to each other.

![ERD Cardinality Symbols ](https://drive.google.com/uc?export=view&id=11I2M3DO1OAARfN6PnYia7z0aO9PkgRpT)
<br>

 - **Entity -->**  - A person, organization, objects type, or concept about which information is stored. Can be considered as as the name of the table.
 
|_Strong Entity_ | _Weak Entity_ |
|------------- |---------------|
|`A strong entity is not dependent on any other entity in the schema| A weak entity is dependent on other entity in the schema |
|Will always have primary key| Uses Parent Table Primary key as its own Primary key which is referenced using Foreign Key|
|Represented by Rectangle |Represented by concentric Double Rectangle| 


 - **Fields-->** The information about the entity consisting of different stuffs. for eg for person entity, age, gender, name which tells more about the entity are fields on the entity. 
 
 |_Multivalued Attributes_ | _Derived Attributes_ |
|------------- |---------------|
|A multivalued attribute **may have one or more values for a particular entity| A derived attribute is an attribute whose values are calculated from other attributes |
| A typical example of a composite attribute is a person's address, which is composed of atomic attributes, such as City, Zip, and Street| A example for derived attribute can be a age column which can be derived from the DOB column.|
|Represented as Eclipse |Represented as dotted Eclipse|

 - **Relationship-->** It can be defined as the way the two or more entity are linked to each other. 

### Cardinality representation:
<center>
<img src="https://drive.google.com/uc?export=view&id=12iIbzuEFraw-qYYaA4Qoll2P1K2YyBid" alt="ERD Cardinality" width="700"/>
  </center><br>
  
#### Degree of Relationship
The degree of a relationship is the number of entity types that participate(associate) in a relationship. 

### Types of Relationship.
There are basically 3 Types of Relationship.

 1. **_One-To-One_**:One-to-one relationships associate one record in one table with a single record in the other table.
 2. **_One-To-Many/Many-To-One_**: One-to-many relationships associate one record in one table with many records in the other table
 3. **_Many-To-Many_** : A _many_-to-_many relationship_ occurs when _multiple_ records in a table are associated with _multiple_ records in another table.

### Below is the Diagram for the Relationship
![Relationship-Diagram](https://drive.google.com/uc?export=view&id=1gHRxP55vHaknRRNxDfLCGyrWeplCM0qh)






---
---
You can use the [www.lucidchart.com](https://www.lucidchart.com/pages/ER-diagram-symbols-and-meaning/#discovery__top) tool to draw the ER-diagram at ease and export/publish in variety of formats.
The lucidchart also provides impressive features like providing the SQL written code of the made ERD.

