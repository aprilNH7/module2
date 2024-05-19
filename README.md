# module2

# Overview
This project is a prerequisite for Milestone One and involves using JavaScript skills to refactor the website code based on the client wireframe. The goal is to organize the default code and folder layout into a structure that reflects a Model View Controller (MVC) approach to software design.

# Templating with Handlebars (HBS)
Handlebars (HBS) is a templating system used to build views dynamically, offering extensibility and minimal logic. You will apply HBS and MVC to produce efficient code that renders a website quickly.

# Prompt
Follow the instructions in the Module Two Full Stack Guide. Refactor the HTML Travlr website using the MVC pattern by adding routes and controllers. Ensure the website aligns with the customer requirements from the wireframe description. Implement HBS templates to convert static pages to dynamic ones and insert HBS directives to enable rendering of the views.

# Instructions

# Git Branch Creation
Open a PowerShell window in the Travlr project directory.
Create a new branch for Module Two:
git checkout -b module2

# Web Application Folder Structure
Create an app_server folder in the Travlr project directory.
Move the existing routes and views folders into the app_server folder.

# Creating Controllers and Routes
In the app_server folder, create a folder named Controllers.
In the Controllers folder, create a file named main.js for the main controller.
Edit main.js to serve the main index page.
Update the index.js file in the routes directory to pass the request for the site’s default starting page to the new main controller.
Create a controller for the travlr page following the same steps used for the main controller.
Add a route for the travlr controller.
Edit the app.js file to add the app_server folder to the application path and wire the travlr controller to the route for the /travel page.

# Creating Handlebars Views
Copy travel.html from the public folder to the app_server/views folder and rename it travel.hbs.
Create a partials folder under views and add header.hbs and footer.hbs for header and footer partials.
Replace the common header and footer code in travel.hbs with Handlebars partial references:
{{> header }}
{{> footer }}
Create a layouts subfolder under views and move the layout.hbs file into it.
Edit app.js to register the partials directory with the templating engine.

# Testing
Restart your web server using the command:
npm start
Check the webpage to ensure dynamic content is served correctly.

# Finalizing Module Two
Add all changes to Git tracking:
git status
git add .
git commit -m 'Module 2 completed baseline'
Push the changes to GitHub:
git push --set-upstream origin module2
