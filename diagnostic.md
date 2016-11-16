# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```bash
The purpose of the back end is to take the requests from the front end, complete
the processes involved with those requests (i.e. update a table or delete a line
item), and then to save that change in the database so that change will be
reflected in the future. After all of this the backend sends the front end
the requested information. The backend communicates with servers in order to
track information and change data.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
The model layer should fetch the data, the controller layer should query the
model for that data.
```

Which layer in the MVC pattern communicates with the model?

```bash
The conroller layer communicates with the model. The controller instructs
the model to make the approrpiate changes and then passes the info to the
view layer to be disaplyed after the model layer has completed its processes.
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
Because views are simiply the visualization of the information, they dont
contribute much in regards to information processing or conversaion.
They simiply display the information given to them by the controller.
```

What does C.R.U.D stand for?

```bash
Create
Read
Update
Delete
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bashcd
Controller
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```bash
GET
POST
PATCH
DELETE
UPDATE
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
1. The server must be expecting the data in a certain format. If the request is
sent to the server in the proper format, the server can then begin processing
the request.

2. Next, the server looks for the appropriate page value ('/people/') and then looks for
the appropriate value ('1').

3. Should the server find both, it will then construct the URL and send it back
to the user in the form of a page. 
```

What is the command to generate a new rails-api app?

```bash
rails g scaffold
```

What is the command to start an instance of a rails server?

```bash
rails server
```

What are the commands to drop, create and migrate a database from the command
line? (3 bullet points)

```bash
bundle exec db:drop
bundle exec db:create
bundle exec db:migrate
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
rails g scaffold Pets name:string age:integer
```
