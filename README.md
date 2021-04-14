## A simple API CRUD make with Laravel 8

### Clone the repository
```
$ git clone https://github.com/drbarzaga/api-crud-laravel8.git
```

### Setup the environment
 Please copy the .env.example to .env and set the environment variables here.
 
```
$ copy .env.example .env
```

### Install dependencies
```
$ composer install
```

### Run Migrations
```
$ php artisan migrate
```

### Run Development Server
Move to the project directory and run this command to start the development server.
```
$ php artisan serve
```

### Testing API
For testing the API endpoints you use the Postman Collection that appears in the repository.
The collection contains an environment named ```API CRUD Laravel8``` feel free for edit the
environment.

![API CRUD Laravel8 Environment](/public/images_doc/environment.png)

### Security End Points
- Register an user
```
POST api/register
```
![Register User](/public/images_doc/register.png)

- Login
```
POST api/login
```
![Login](/public/images_doc/login.png)

### Projects End Points
- List Projects 
```
GET api/project
Authorization: Bearer Token
```
![List Projects](/public/images_doc/list_projects.png)

- Create Project
```
POST api/project
Authorization: Bearer Token
```
![Create Project](/public/images_doc/new_project.png)

- Project Details
```
GET api/project/:project_id
Authorization: Bearer Token
```
![Project Details](/public/images_doc/show_project.png)

- Edit Project
```
PUT api/project/:project_id
Authorization: Bearer Token
```
![Edit Project](/public/images_doc/edit_project.png)

- Delete Project
```
DELETE api/project/:project_id
Authorization: Bearer Token
```
![Delete Project](/public/images_doc/delete_project.png)