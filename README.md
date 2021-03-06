# T3A2 - A

#### Deployed site

Access to Homepage and booking form is on https://cleaning-management.netlify.app/
Access to Admin and Employee login is on https://cleaning-management.netlify.app/dashboard

Backend api - https://cleaning-managment-api.herokuapp.com/
#### Repositories

Github Backend - https://github.com/T3A2-DreamTeam/Cleaning-Management-Backend
Github Frontend - https://github.com/Brayydzz/Cleaning-Management-Frontend

## **Purpose & Target Audience:**

Our purpose is to build a full-stack application to assist a local cleaning business handle and manage her employees & clients. The application allows The employer to assign and delegate cleaning jobs to their employees via a Employee job page. Employee can view all of their assigned tasks and once they have completed a job, they can assign the job as complete and write any notes required for that job. Clients contact the employer via the contact page. The employer will assign and mage those tasks to a specific employee. The target audience for this application is for a business owner of a cleaning business needing an easier way to manage both their clients and employees.

## **Features:**

Clients can send a booking request through the Contact Page

Admin/Employer Can review all incoming bookings and delegate jobs to their employees

Admin/Employer can view all of their employees current jobs/availabilities

Admin/Employer can view all previous jobs and clients

Admin/Employer is able to view which current employees are available to be assigned a job

Employees can view all of there current delegated jobs

Employees Can complete jobs via a job page and add notes to the completed job

## **User Stories:**

User stories can be found here on our Trello board - https://trello.com/b/1G3kz4wC/t3a2-cleaning-service

## **Tech Stack:**

- Javascript
- React
- Ruby on Rails
- Cloudinary
- Postgres
- Netlify
- Heroku
- CSS

### **Node Packages:**

### Cypress

Cypress is a testing framework that is based in Javascript and is used for end to end testing. It allows developers to perform asynchronous tests easily inside of a testing shell.
We used Cypress testing to run automated and manual tests in our front end environments. Checking inputs, buttons, alerts and redirects.

### dotenv

Dot env allows us to create a '.env' file to save environmental variables to load them in where needed without having to hardcode values and allows us to have secret keys stored in one place and not in the code to push to github.

### jwt-decode

JWT is used to decode and encode tokens to allow users to sign in and authenticate, as well as authorization. A ruby implementation of the RFC 7519 OAuth JSON Web Token (JWT) Standard (https://datatracker.ietf.org/doc/html/rfc7519).
In the application controller we have made a few auth functions to help with this. There is a method for checking if someone is logged in, a method to decode the incoming token, a method to return the user that is logged in and a method to see if the person logged in is an admin.

### react-icons

React Icons is a simple package that has a whole library of popular icons to use in your react Project. These Icons were implemented for the responsive mobile Navbar.

### react-modal

React Modal is an easy to use package that allows you to implement a Modal component. It was used in our user Dashboard to view more information on Employees, Clients and Jobs.

### react-responsive-carousel

React responsive carousel is a package that allows you to implement an easy to use and customizable image carousel. The carousel was used within the job modal for the user to view images that have been uploaded to a job.

### react-router-dom

react-router-dom is way to allow for dynamic, client-side routing. It helps us to develop a single-page web application with navigation without the need for the page to refresh as a user navigates through the site.
We heavily rely on react-router throughout the front-end of the application and it can been seen in the App component.

### react-select

React Select is a simple package that allows you to implement a searchable select box. This was used to search through Clients and Employees when assigning them to a job.

### styled-components

Styled components is a package that allows you to export reusable styled components throughout your react application. These styled components were used for the majority of styling throughout our app.

### validator

### **Ruby Gems:**

### Bcrypt

Bcrypt is used for hashing passwords. Rails uses bcrypt with the keyword.
Bcrpyt is a hashing algorithm designed by Niels Provos and David Mazi??res of the OpenBSD Project. Hash algorithms take a chunk of data (e.g., your user's password) and create a "digital fingerprint," or hash, of it. Because this process is not reversible, there's no way to go from the hash back to the password.
Within Bcrypt we utilize password_digest in our User Model. This stores the password safely and when retrieving User data it will filter out the password for security reasons.

### Cloudinary

"Cloudinary is a cloud service that offers a solution to a web application's entire image management pipeline. It can easily upload images to the cloud. Automatically perform smart image resizing, cropping and conversion without installing any complex software. Integrate Facebook or Twitter profile image extraction in a snap, in any dimension and style to match your website???s graphics requirements. Images are seamlessly delivered through a fast CDN, and much much more.
Cloudinary offers comprehensive APIs and administration capabilities and is easy to integrate with any web application, existing or new.
Cloudinary provides URL and HTTP based APIs that can be easily integrated with any Web development framework.
For Ruby on Rails, Cloudinary provides a GEM for simplifying the integration even further."

We implemented Cloudinary in our app to give the functionality to be able to attach images to a job. This allows the employees and admin to pass information about the job that would otherwise be difficult.
We have hard coded the limit for the amount of images of a job to 10 images so to avoid having the image database being abused.

### JWT

JWT is used to decode and encode tokens to allow users to sign in and authenticate, as well as authorization. A ruby implementation of the RFC 7519 OAuth JSON Web Token (JWT) Standard (https://datatracker.ietf.org/doc/html/rfc7519).
In the application controller we have made a few auth functions to help with this. There is a method for checking if someone is logged in, a method to decode the incoming token, a method to return the user that is logged in and a method to see if the person logged in is an admin.

### Dotenv

Dot env allows us to create a '.env' file to save environmental variables to load them in where needed without having to hardcode values and allows us to have secret keys stored in one place and not in the code to push to github.

#### References

https://github.com/cloudinary/cloudinary_gem
https://github.com/jwt/ruby-jwt
https://github.com/bcrypt-ruby/bcrypt-ruby

### **Manual Testing:**


Admin login:
email - a@b.com
password - password

Employee login:
email - a@b.c
password - password

created employee logins
email - employee email
password - Passw0rd!

_Please use Chrome as a Web Browser_

Access to Homepage and booking form is on https://cleaning-management.netlify.app/
Access to Admin and Employee login is on https://cleaning-management.netlify.app/dashboard

### **Project Management/Task Delegation**

In our full-stack web application project we started by having a discussion about our individual strengths and weaknesses and then divided our work load between our group depending on those strengths. Essentially the work was divided into three main parts where each team member would focus on one main aspect. Front-end development which focused primarily on React framework and included importing npm packages, creating and implementing components, and styling. Back-end development which focused primarily on the Rails framework and included installing gems, creating models and controllers, organizing the database and implementing third party servers like Cloudinary. Testing and documentation which focused on implementing tests for both front and back-end frameworks, hard coding JSX text for the site, creating dummy data such as seeds for the database and recording the necessary documentation for the project.
We utilized a Trello board to keep track of our job boards with achievable goal dates. And we conducted our own informal stand-ups each morning where would discuss current progress, outstanding issues and then outline the tasks for the day. Throughout the development of the application we found that the back-end was easier to implement than the front-end. In this case our back-end team member assisted our front-end developer with more difficult logic to allow them more freedom to bulk the project out.
