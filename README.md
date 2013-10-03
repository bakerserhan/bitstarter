Output of the tree command, with line-by-line annotations as to what the files do.


```
|-- .env.dummy      # Template for .env; use to keep private API keys out of git repo<br/>
|-- .pgpass         # Username/password file for local Postgres install<br/>
|-- .gitignore      # Define files (like .env) that won't be committed to git<br/>
|-- Procfile        # Specify what script is run on Heroku<br/>
|-- README.md       # Markdown documentation; formatted for github<br/>
|-- index.html      # Main page, with CSS/JS/img assets imported via link<br/>
|-- models         <br/>
|   |-- index.js    # Instantiate db object, connect to remote/local postgres<br/>
|   |-- order.js    # Mapping between Postgres table and fields of Order JS object<br/>
|-- package.json    # Define which npm modules are needed; used for Heroku deploy<br/>
|-- pgsetup.sh      # Set up local Postgres db from .pgpass for use by index.js<br/>
|-- setup-ssjs.sh   # Set up npm, heroku, and postgres for the app to run<br/>
|-- views          <br/>
|-- orders.ejs  # template for displaying Order instances as HTML<br/>
|-- web.js          # Main express app; defines /, /order, and /refresh_order routes<br/>
```
