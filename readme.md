# Individual Assignment: Portfolio Website

## Objective
In this assignment you will be creating your own personal portfolio website! This project will give you a chance to showcasing your experience and projects as a student developer.

While building your portfolio you will learn to structure a web application following the Model-View-Controller (MVC) architecture. You will also gain practical experience defining clean and easy to understand web URLs. The pages that comprise your portfolio will be built using a templating engine — either Pug or EJS — which will make it easier to write HTML pages as well as provide dynamic pages.

## Setup and Configuration
Start by initializing a new Node.js project with `npm init` and install necessary packages: 

1. `express` - You will be using Express.js for the project.
2. `pug` or `ejs` - Pick whichever templating language you like. 
3. `nodemon` - To make debugging easier.

Set up an Express server to listen on a suitable port.

## Directory Structure
Your project should be organized into the following logical directory structure:
- `controllers` for routing requests and business logic
- `views` for HTML templates
- `models` if necessary, though not required here
- `public` for static files like CSS, JavaScript, and images
- `data` to house the `projects.json` file

## Routing and Pages
Define routes in your Express application that render pages through the templating engine. All routes should begin with the `/portfolio` path:
- **Home/About Me** (`/portfolio` or `/portfolio/about`): This route will serve as the landing page providing a brief introduction about the student.
- **CV** (`/portfolio/cv`): This route will display the student's curriculum vitae or resume.
- **Personal Projects** (`/portfolio/projects`): This route will dynamically render a list of projects stored in `projects.json`. Each project's details should be read from the file and passed to the view template to be displayed.
- **Personal Projects** (`/portfolio/projects/:id`): This route will show a single project whose id matches the path variable.

Note: All of the HTML pages described above should be located in the views directory.

## Templating
You are free in this assignment to choose Pug or EJS to create templates for each page. Templates should utilize a consistent layout across all pages, with a shared navigation system. The CSS stylesheets provided should provide a modern and professional look.

Note: Low effort submissions in terms of styling will be graded down.

## Static Files
Configure Express to serve static files from the `public` directory. This ensures that any CSS, JS, image, or other static files can be directly referenced in your view templates.

## Dynamic Content
To support the Personal Projects page, you should create a `projects.json` file in the data directory. Pass this data to the view, where it will be used to dynamically generate content about each project.

## MVC Architecture
- **Model**: While a formal model isn't necessary for this simple data structure, consider creating a module to handle reading and parsing the JSON data if you want to introduce some basic data handling concepts.
- **View**: Use the templating engine to manage the HTML output.
- **Controller**: Create controllers for handling the routing logic, including fetching data for the projects.

## Documentation and Submission
Include a `README.md` file detailing the project setup, structure, and any necessary instructions on how to run the website.

## Evaluation Criteria
Students will be evaluated based on the functionality of the routes, the quality and organization of the code, and the design and usability of the website.