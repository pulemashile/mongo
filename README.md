MongoDB Setup and Basic Operations Guide
Introduction
This guide will help you set up MongoDB and perform basic  operations such as inserting documents in a newly created database called codetribes.

Prerequisites
Before proceeding, ensure you have:

MongoDB installed on your local machine or use MongoDB Atlas for a cloud-based setup.
MongoDB Shell or MongoDB Compass (GUI for MongoDB).

Basic understanding of JSON-like documents.
Steps
1. Install MongoDB
Follow the installation instructions from the official MongoDB documentation:

MongoDB Installation Guide
2. Start MongoDB
Start the MongoDB server:

bash
mongod
This will run the server locally on port 27017 by default.

3. Connect to MongoDB
Open a new terminal window and start the MongoDB shell by running:

git bash

mongosh
You will see the MongoDB shell prompt (>) where you can interact with your database.

4. Create a Database: codetribes
To create and switch to the codetribes database, use the use command:
use codetribes
MongoDB will automatically create the database when you first insert data.

5. Create Collections and Insert Data
MongoDB collections are created automatically when you insert data. Below are the steps to insert sample data into three collections: Trainees, Project, and Facilitator.

Insert Data into the Trainees Collection


db.Trainees.insertOne({Name: "fifi", Location: "Polokwane", Facilitator: "sizwe"})

Insert Data into the Project Collection


db.Project.insertOne({Name: "App", Course: "IT", Lesson: "Introduction to CSS"})
Insert Data into the Facilitator Collection
javascript

db.Facilitator.insertOne({Name: "Sizwe", Location: "Polokwane", Course: "React"})

6. Verify Data Insertion
You can verify that data was inserted correctly by running the following queries:

View all data in the Trainees collection:

db.Trainees.find()
View all data in the Project collection:

db.Project.find()
View all data in the Facilitator collection:


db.Facilitator.find()

# mongo![creatingdatabase](https://github.com/user-attachments/assets/5120d642-e99b-404e-ad9b-899654b550f3)
