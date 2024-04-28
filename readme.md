# Portfolio Website using Node.js and Express

## Objective
Develop a personal portfolio website showcasing your skills and projects. The website will use Node.js and Express.js, along with a templating engine like Pug or EJS. It will follow the MVC architecture to organize the code.

## Setup and Configuration
Start by initializing a new Node.js project with `npm init` and install necessary packages such as `express`, and your choice of `pug` or `ejs`. Set up an Express server to listen on a suitable port.

## Directory Structure
Create a logical directory structure:
- `controllers` for business logic
- `views` for HTML templates
- `models` if necessary, though not required here
- `public` for static files like CSS, JavaScript, and images
- `data` to house the `projects.json` file

## Routing and Pages
Define routes in your Express application that render pages through the templating engine:
- **Home/About Me** (`/` or `/about`): This route will serve as the landing page providing a brief introduction about the student.
- **CV** (`/cv`): This route will display the student's curriculum vitae or resume.
- **Personal Projects** (`/projects`): This route will dynamically render a list of projects stored in `projects.json`. Each project's details should be read from the file and passed to the view template to be displayed.
- **Technology Interests** (`/tech`): This route will show a list or detailed descriptions of the technologies the student is interested in.

## Templating
Use Pug or EJS to create templates for each page. Templates should utilize a consistent layout incorporating shared elements like headers and footers through partials.

## Static Files
Configure Express to serve static files from the `public` directory. Ensure to include CSS for styling the website.

## Dynamic Content
Particularly for the Personal Projects page, implement logic in the controller to read from `projects.json`. Pass this data to the view, where it will be used to dynamically generate content about each project.

## MVC Architecture
- **Model**: While a formal model isn't necessary for this simple data structure, consider creating a module to handle reading and parsing the JSON data if you want to introduce some basic data handling concepts.
- **View**: Use the templating engine to manage the HTML output.
- **Controller**: Create controllers for handling the routing logic, including fetching data for the projects.

## Documentation and Submission
Include a `README.md` file detailing the project setup, structure, and any necessary instructions on how to run the website.

## Evaluation Criteria
Students will be evaluated based on the functionality of the routes, the quality and organization of the code, and the design and usability of the website.