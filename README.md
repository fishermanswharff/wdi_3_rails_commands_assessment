# Rails Commands Quiz

Fork, clone, and write your answers directly in this file. Then submit a pull request.

### Question 1

I want to start a new Rails project/app called `BunnyApp`. What command should I type in the terminal?
rails new BunnyApp --database=postgresql

### Question 2
<!-- Referenced RailsGuides for this -->
I want to create a new model called `Bunny`, with the following attributes: name (string), color (string), and age (integer). What command should I type in the terminal?
rails g model Bunny name:string color:string age:integer

### Question 3
<!-- Referenced RailsGuides for this -->
What does the command in Question 2 do, exactly? What files are created, where are they located, and what does the database look like at this time? Explain.
the files generated are a db file for mapping our model to a db table, and a model file, called bunny.rb. The db file will have 3 columns slated for inserting into the db table: name, which takes a string, color which takes a string, and age which takes an integer. Our db doesn't look like anything yet because we haven't run rake db:migrate.

### Question 4

I want to create a database and make it reflect the new model I created in Question 2. What command(s) should I type in the terminal?
rake db:migrate

### Question 5

I want to look at the actual database that has been created. What command should I type in the terminal?
rails db, then \d bunny to look at the bunny table.

### Question 6

I want to see a list of all the URLs available in my app, along with the HTTP requests and controllers associated with them. What command should I type in the terminal? 
rake routes

### Question 7

I have worked on my app and finally want to see it in action. What command should I type in the terminal, and where should I navigate to in my browser?
you have to navigate to your project folder in terminal, type rails (s)erver, and navigate to http://localhost:3000. 
