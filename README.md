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
