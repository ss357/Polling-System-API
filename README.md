# Api-Polling-System

## Introduction

Creating a **Polling System API** where anyone can create questions with options and also add votes to it. It is built
using Express, Nodejs, MongoDB.

<br/>

## Features

- Users can create questions (you can add as many questions as you want).
- Users can add options to a question.
- Users can add a vote to an option of question.
- Users can delete a question -> A question can't be deleted if one of it's options has votes.
- Users can delete an option -> An option can't be deleted if it has even one vote given to it.
- Users can view a question with it's options and all the votes given to it.

## Routes & URL

- **/questions/create**
  <p> To create a new question hit the following URL with a post request:</p>
  https://polling-system-api-517c.onrender.com/api/v1/questions/create

- **/options/:id/create**
  <p>To create a new option for a question hit the following URL with a post request:</p>
  https://polling-system-api-517c.onrender.com/api/v1/questions/:idOfQuestion/options/create

- **/options/:id/addVote**
  <p>To increment the count of votes on an option, hit the following URL with a get request:</p>
  https://polling-system-api-517c.onrender.com/api/v1/options/:idOfOption/addVote

- **/questions/:id**
  <p> To view a question and it’s options, hit the following URL with a get request:</p>
  https://polling-system-api-517c.onrender.com/api/v1/questions/:idOfQuestion

- **/options/:id/delete**
  <p> To delete an option, hit the following URL with a delete request: </p>
  https://polling-system-api-517c.onrender.com/api/v1/options/:idOfOption/delete

- **/questions/:id/delete**
  <p> To delete a question, hit the following URL with a delete request: </p>
  https://polling-system-api-517c.onrender.com/api/v1/questions/:idOfQuestion/delete
  <br/>

- Version Control System: Git
- VCS Hosting: GitHub
- Integrated Development Environment: VSCode
  <br/>
  <br/>

## Requirements

For development, you will only need Node.js and a node global package installed in your environement and mongodb for database.

### Node

- Node Installtion on Windows
  Go on to the [official Node.js website](https://nodejs.org/en/) and download the installer. Also, be sure to have `.git` available in your PATH,
  `npm` might need it (You can find [git](https://git-scm.com/)).
- Other operating System
  You can find more information about the installation on the official [Node.js website](https://nodejs.org/en/) and the official [NPM website](https://www.npmjs.com/).

If the installation was successful, you should be able to run the following command.

```
$ node --version

$ npm --version
```

If you need to update `npm`, you can make it using `npm`! Cool right? After running the following command, just open again the command line and be happy.

```
$ npm install npm -g

```

<br/>

## To run the project on your local machine:

1. Open terminal.

2. Change the current working directory to the location where you want the cloned directory.

   ```
   $ git clone https://github.com/ss357/Polling-System-API.git

   ```

3. Install all the dependencies by running :

   ```
   npm install

   ```

4. Run npm start to run the project at local host, port 8000:

   ```
   $ npm start

   ```
