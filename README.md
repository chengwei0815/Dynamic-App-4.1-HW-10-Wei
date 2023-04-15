CP: Homework #10
Completion requirements
Opens: Saturday, 15 April 2023, 2:00 PM
Due: Monday, 24 April 2023, 11:59 PM
Objectives
Taking the information that we have learned from 5.0 - Intro to Back End Development and Period 1 of this unit, we will install Node.js, reorganize our directory structure so that it will slowly have an MVC Architecture, have a few GET routes to explore how we can create http request and response, and start a Node.js server.

Directions
Make sure you are in the homework-9 branch of your course project in VS Code. Create a new branch called homework-10, and do all the work for this assignment in the homework-10 branch.

Installing Node.js and dependencies
Create a new file called app.js. Make sure that this file is at the root of your directory
Inside of your terminal, type in the following to start a Node project: npm init. Answer all the prompts until completion. Remember that app.js is replacing the index.js that it suggests
Next, install all the following dependencies that will be needed for the project: npm install express ejs mongoose dotenv morgan method-override
Then install all the dependencies needed only for development: npm install nodemon uuid --save-dev
In VSCode, open the package.json file and add the following code within the script object:
"dev": "nodemon app.js",
Preparing the Directory Structure to be a Node.js Project
In the root directory, make a new directory called views
Inside of the views directory, make another directory called pages
Move all of the HTML files into the pages directory
In the root directory, add the gitignore-file.txt that is attached to this assignment. Rename it to be .gitignore with no file extension
Make sure that you still have a public directory that contains three directories: images, scripts, and styles. If you don't have this, make sure to organize your directory now. At the end of reorganizing, your structure should look like this:

Directory Structure

Starting the Node.js server
In your VSCode, open app.js
First, require the following dependencies: express and morgan
Create a const variable called app with the value of express()
Create a const variable called port with the value of 3000
Use morgan as a middleware for this project
Create five  basic GET routes with the following information
PATH: /, HANDLER: "This route points to the Home page"
PATH: /about, HANDLER: "This route points to the About page"
PATH: /login, HANDLER: "This route points to the Login page"
PATH: /admin-console, HANDLER: "This route points to the Admin Console page"
PATH: /admin-console/create-book, HANDLER: "This route points to the Create page"
use app.listen() to start the server and send a console.log to the terminal with the localhost URL
Run server and test routes
start server by running npm run dev
test localhost in browser
Push your work to Github
Do your Git workflow and push your work to homework-10 repo on Github
Merge homework-10 to your main or master branch
Push main or master branch to Github

gitignore-file.txt gitignore-file.txt24 October 2022, 12:46 PM
