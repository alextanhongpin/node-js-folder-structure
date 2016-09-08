# Node JS Folder Structure

### Some best practices in structuring a large node js project folder.

```
|app.js
|package.json
|--app
|   |--models
|        |--user.js
|        |--user-schema.js
|   |--views
|   |--controllers
|--config
|   |--authentication.js
|   |--credentials.js
|   |--routes
|        |--page_1.js
|        |--page_2.js
|        |--login.js
|        |--signup.js
|   |--database.js
|   `--locale
|        |--en_us.js
|--public
|   |--controllers
|--react
|   |--atoms
|        |--button.jsx
|        |--button.sass
|        |--button-responsive.sass
|   |--molecules
|   |--organisms
|   |--templates
|   |--pages
|--views
|   |--layouts
|   |--pages
|--tests
|   |--users
|   |--admins
```
+ Folder naming can be singular or plural, but should be standardized
### Root folders:
+ *app* - holds the whole express code structure
+ *public* - holds the static file. Best if server using a CDN.
+ *views* - contains the static html views

### App folder contains the following:
+ *models* - contains the schema for the models and database
+ *routes* - contains the express js routes
+ *stores* - database access layer code
+ *configs* - holds the whole app configuration, including routes endpoints, auth and database config
+ *helpers* - a.k.a. useful utils
+ *middlewares* - the heart of express

### API folder will contain the following:
+ *entity* - the request params, including validation
+ *graph* - helper to parse the response
+ *action* - config for the services which contains the method, routes, and commands to be dispatcher
+ *command* - triggered by command to handle a specific requests
+ *store* - database access layer

### Deciding factor for the app architecture
+ how reusable is it from the scale of 1 to 10?
+ how granular should the files be? preferable 150 loc (line of codes) per file
+ each file does only one thing best
+ reusable codes are extracted out


## Client side folder structure

+ is separated from the server side
+ communicates with the server side through REST calls or websocket

###Folder Structure:
+ assets (including images, fonts, etc)
+ scripts (we do not choose js owing to the variety of compilers available now such as coffeescript, jsx, etc and thus do not want to be tied to a specific technology)
+ stylesheets (css, less, sass files resides here)
+ data (static data)
