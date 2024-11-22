<img src="https://socialify.git.ci/Asanda001019/Task21-MongoDb-Databases-Collections-Documents/image?font=Rokkitt&language=1&name=1&owner=1&pattern=Brick%20Wall&stargazers=1&theme=Dark" alt="Task21-MongoDb-Databases-Collections-Documents" width="640" height="320" />
<h1>Task21-MongoDb-Databases-Collections-Documents</h1>h1>
<p>MongoDB Task: Codetribe Database
Overview
The Codetribe Database project involves creating a MongoDB database and managing collections and documents for a fictional organization called "Codetribe." This task covers creating and understanding databases, collections, and documents in MongoDB, along with exporting the database and pushing it to GitHub.

Key Concepts
Databases: MongoDB organizes data into databases.
Collections: Collections are groups of documents within a database.
Documents: MongoDB stores data in JSON-like documents that are flexible and can have various data types (including arrays, embedded documents, and more).
Objectives
Create and manage MongoDB databases, collections, and documents.
Understand and differentiate between JSON and BSON (Binary JSON).
Use MongoDB shell commands to create a database, insert data, and export it.
Instructions
1. Run MongoDB Locally
Follow these steps to get the MongoDB shell running locally:

Start MongoDB Shell: To start the MongoDB shell, open your terminal and type the following command:

bash
Copy code
mongosh
Create the Codetribe Database: Switch to the Codetribe database. If it doesn’t exist, MongoDB will create it for you once you insert some data:

bash
Copy code
use Codetribe
Create Collections and Insert Documents: MongoDB stores data in collections. Below are the collections to be created:

Facilitators collection: Insert a document with the fields Name, Location, and Course.

bash
Copy code
db.Facilitators.insertOne({
  Name: "Dlozi Mthethwa",
  Location: "Johannesburg",
  Course: "Graphic Designer"
})
Trainees collection: Insert a document with the fields Name, Location, and Facilitator.

bash
Copy code
db.Trainees.insertOne({
  Name: "Asanda Madondo",
  Location: "Richmond",
  Facilitator: "Mr Mthethwa"
})
Projects collection: Insert a document with the fields Name, Course, and Lesson.

bash
Copy code
db.Projects.insertOne({
  Name: "MongoDB Introduction",
  Course: "MongoDB Basics",
  Lesson: "CRUD Operations"
})
2. Export the Database
To export the Codetribe database, use the mongodump command:

Exit MongoDB Shell: Type exit to leave the MongoDB shell.

bash
Copy code
exit
Run the Export Command: In your terminal, run:

bash
Copy code
mongodump --db=Codetribe --out=./CodetribeExport
This will create a backup of your Codetribe database in the CodetribeExport folder.

3. Push to GitHub
To push the exported database and the README file to GitHub:

Initialize a Git repository (if not already initialized):

bash
Copy code
git init
Add your files to the Git repository:

bash
Copy code
git add .
Commit your changes:

bash
Copy code
git commit -m "Initial commit with Codetribe database and README"
Add your GitHub repository:

bash
Copy code
git push -u origin master
Tech Stack
Client: MongoDB, MongoDB Shell
Tools: Command Line Interface (CLI), GitHub, Git</p>
