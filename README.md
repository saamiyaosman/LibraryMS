# Library Management System
[Link to: Jira Board](https://saamiyaosman.atlassian.net/jira/software/c/projects/DFE/boards/2)
## Initial Questions
##### Why are we doing this?
I am doing this project to implement the Java we have learnt into a practical application hence I've created my Library MS.

##### How I expected the challenge to go. 
I expected to get my program to be fully functional with some custom queries and relevant tests to also be included.

##### What went well?
I managed to create the MVP for this project so the Library MS can do all the CRUD functionality via Postman as well as all the tests for them have passed. Plus I managed to get testing to hit over 80% coverage.

##### What didn't go as planned? 
During this project I tried to add a custom query that would check if a book being created already existed and if it did would add 1 to the quantity. Whe I tried to implement this method I could not get it t work and ultimately since it ws dependant on other queries some of the CRUD functions that were previously working started to throw up errors. Plus I had some issues with my branches since I was trying to get used to using a feature branch model and sometime would end up pulling branches back to the dev when I was not intending to.

##### Possible improvements for future revisions of the project. 
I would try to re-implement my custom query and a few other queries I wanted to add but did not get the time to do. Plus, I would try to add a front end instead of just using Postman to run my queries.

## Postman, API and Database Functioning
### CREATE
#### Postman Request
This screenshot shows the Postman request adding a new book to the library and the API returning the value as its stored in the database(thus all the data alongside its primary key value).

![Screenshot (17)](https://user-images.githubusercontent.com/98022076/158997473-f25468dd-179d-4d11-9ca3-135da02046e8.png)

#### Changes to the Database
This is what the database looked like before the query.

![Screenshot (37)](https://user-images.githubusercontent.com/98022076/159002439-59f24033-8aa3-40e0-bc39-2c677a084b52.png)

As a result the new record has been added to the database as shown in the screenshot below.

![Screenshot (19)](https://user-images.githubusercontent.com/98022076/158998144-773a7267-7580-4f41-a9cb-6496a932445e.png)


### READ
#### Postman Request
This screenshot shows the Postman request reading all the values from the library database and the API returning all the values onto the console.

![Screenshot (21)](https://user-images.githubusercontent.com/98022076/158998680-c95d270e-23ed-4ef0-a447-da559770f974.png)

#### Changes to the Database
This command is a GET command so does not persist any changes to the database.


### READ BY BOOKID
#### Postman Request
This the postman request reading the record for the specific bookId from the database via a path variable and the API returning the value onto the console.

![Screenshot (23)](https://user-images.githubusercontent.com/98022076/158999403-795a9400-08be-4516-9263-b11bbc337901.png)

#### Changes to the Database
This command is a GET command so does not persist any changes to the database.


### UPDATE
#### Postman Request
This the postman request requesting to change the quantity from 8 to 7 in the database and the API returning the record with the new value into the console.

![Screenshot (25)](https://user-images.githubusercontent.com/98022076/158999957-3f1c6454-87cb-4f50-8330-c131266f4c7b.png)


#### Changes to the Database
This is the old record in the database looked like with quantity value 8.

![Screenshot (31)](https://user-images.githubusercontent.com/98022076/159001449-69a61332-aa9b-47ef-9a33-462152afad66.png)

This is the new record in the database with the quantity altered to 7.

![Screenshot (27)](https://user-images.githubusercontent.com/98022076/159000706-ee96bf51-9391-48a0-9ca1-ed754e7b8f76.png)

### DELETE
#### Postman Request
This the postman request to delete bookid 8 from the database and the API returning the deleted value in the console.

![Screenshot (33)](https://user-images.githubusercontent.com/98022076/159001741-52aa4bad-177a-4cc8-a144-63a4c8c2096a.png)

#### Changes to the Database
This is the record in the table before the query is run.

![Screenshot (27)](https://user-images.githubusercontent.com/98022076/159000706-ee96bf51-9391-48a0-9ca1-ed754e7b8f76.png)

This is the table after the query is run and bookId 8 has been deleted.

![Screenshot (35)](https://user-images.githubusercontent.com/98022076/159002226-18e49431-11ca-4195-b62d-4bda84828c06.png)

## Testing
### Test Results
Testing and refactoring of the code is in the documentation folder and final test reults are in the screenshot below.

![Screenshot (15)](https://user-images.githubusercontent.com/98022076/158997149-b8415838-3225-47ec-9354-99a46a891ce3.png)

### Coverage
I've added my coverage report in the following screenshot.

![Screenshot (14)](https://user-images.githubusercontent.com/98022076/158985333-9bb4a428-b7e5-401a-b2bd-b60265f55e00.png)
