# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
The backend allows for persistence of data and it allows us to validate everything coming from the client.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
Model
```

Which layer in the MVC pattern communicates with the model?

```md
Controller
```

Why don't we use views in our interpretation of the MVC pattern?

```md
We do not use views because we are building an API, not a web app.
```

What does C.R.U.D stand for?

```md
Create, Read, Update, Destroy
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
I'm slightly confused by this question.

The controller calls the CRUD actions but the model is where the CRUD methods themselves are.
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
#index
#show
#update
#create
#destroy
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
- The router parses the http request
- The router calls the appropriate controller action
- The controller consults the model to get the required data
- The controller responds to the client with the requested data
```

What is the command to generate a new rails-api app?

```bash
rails new <app_name> --api
```

What is the command to start an instance of a rails server?

```bash
bin/rails server
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
bin/rake db:drop db:create db:migrate db:seed
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
bin/rails generate scaffold pet name:string age:integer
```
