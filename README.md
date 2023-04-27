# Design and Development of a Database for a Travel Agency

This is one of my university projects where I practiced in prototyping and developing a database for a travel agency, adding testing data to the DB and writing queries, procedures, and triggers.

## The Idea of the Project
1. Select a business to create a DB for,
2. Dig deeper into what problems this type of business usually faces and how they can be solved with the help of a database,
3. Design and deploy a database based on how this business works,
4. Add testing data to the tables and **provide practical use cases of the database using queries, procedures, and triggers**.

## Tech Stack
1. ERwin Data Modeler - logical and physical modeling
2. Microsoft SQL Server & Microsoft SQL Server Management Studio - deploying the database and working with it

## Results
### Theoretical Part (Data Modeling)
1. The type of business selected was "Travel Agency",
2. After thorough research, it became clear what entities and relationships between them should be added to the database to match the business processes,
3. Firstly, the logical model was created in ERwin Data Modeler, and the structure of the data model was checked for consistency with 3NF,

<img src="https://github.com/maxim-lipatnikov/travel-agency-database-development/blob/main/diagrams/er_logical.JPG" width="700" />

5. After that the physical model of the database was created as well as the script to create all the tables and relationships in Microsoft SQL Server Management Studio (SSMS),

Physical model:

<img src="https://github.com/maxim-lipatnikov/travel-agency-database-development/blob/main/diagrams/er_physical.JPG" width="700" />

Diagram of the database:

![](https://github.com/maxim-lipatnikov/travel-agency-database-development/blob/main/diagrams/db%20diagram.JPG)

7. After the DB was created, testing data was added to all the tables,
8. The second important part of this project was providing use cases of the database based on usual business needs.

### Practical Part (Use Cases of the DB)
#### Queries examples

1. The query returns the number of vouchers sold for each tour with sorting
<img src="https://github.com/maxim-lipatnikov/travel-agency-database-development/blob/main/queries/sold%20vouchers%20for%20each%20tour.png" width="500" />

2. The query returns the number of vouchers sold by each worker of the company
<img src="https://github.com/maxim-lipatnikov/travel-agency-database-development/blob/main/queries/sold%20vouchers%20by%20each%20worker.png" width="500" />

3. The query returns the number of underage cliens
<img src="https://github.com/maxim-lipatnikov/travel-agency-database-development/blob/main/queries/number%20of%20underage%20clients.png" width="500" />

4. The query returns information about the tour bought by family members (in this example, they are just people with similar last name)
<img src="https://github.com/maxim-lipatnikov/travel-agency-database-development/blob/main/queries/family%20members%20with%20one%20last%20name.png" width="500" />

5. The query returns information about what clients bought vouchers for different tours and which workers sold them these vouchers in May 2020
<img src="https://github.com/maxim-lipatnikov/travel-agency-database-development/blob/main/queries/workers%2C%20clients%20and%20tours%20in%20may%202020.png" width="500" />

6. The query returns total revenue from sales of vouchers and number of vouchers sold for a selected tour
<img src="https://github.com/maxim-lipatnikov/travel-agency-database-development/blob/main/queries/total%20revenue%20from%20sales%20of%20a%20certain%20tour.png" width="500" />

7. The query returns the tours with "All inclusive" or "Ultra inclusive" service
<img src="https://github.com/maxim-lipatnikov/travel-agency-database-development/blob/main/queries/tours%20with%20all%20inclusive%20and%20ultra%20inclusive.png" width="500" />

8. The query returns the number of available excursions for each tour
<img src="https://github.com/maxim-lipatnikov/travel-agency-database-development/blob/main/queries/tours%20and%20number%20of%20excursion%20types%20in%20them.png" width="500" />

9. The query returns worker's contact info if his salary is less than 55k RUB
<img src="https://github.com/maxim-lipatnikov/travel-agency-database-development/blob/main/queries/worker%20info%20if%20his%20salary%20less%20than%2055k%20rub.png" width="500" />

10. The query returns contact info of clients who bought vouchers for individual tours
<img src="https://github.com/maxim-lipatnikov/travel-agency-database-development/blob/main/queries/customers%20info%20(individual%20tour%20vouchers).png" width="500" />

### Triggers examples

1. Trigger adds a new empty group for clients if a new group tour as added to the database
<img src="https://github.com/maxim-lipatnikov/travel-agency-database-development/blob/main/triggers/trigger%201%20(add%20new%20empty%20group%20if%20new%20group%20tour%20is%20added).png" width="500" />

Testing:

<img src="https://github.com/maxim-lipatnikov/travel-agency-database-development/blob/main/triggers/trigger%201%20try.png" width="500" />
<img src="https://github.com/maxim-lipatnikov/travel-agency-database-development/blob/main/triggers/trigger%201%20result.png" width="500" />

2. Trigger adds a new empty group for clients if a new group tour as added to the database
<img src="https://github.com/maxim-lipatnikov/travel-agency-database-development/blob/main/triggers/trigger%201%20(add%20new%20empty%20group%20if%20new%20group%20tour%20is%20added).png" width="500" />

Testing:

<img src="https://github.com/maxim-lipatnikov/travel-agency-database-development/blob/main/triggers/trigger%201%20try.png" width="500" />
<img src="https://github.com/maxim-lipatnikov/travel-agency-database-development/blob/main/triggers/trigger%201%20result.png" width="500" />
