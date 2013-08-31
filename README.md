

Output of the tree command, with line-by-line annotations as to what the files do.

.
|-- .env.dummy      # Template for .env; use to keep private API keys out of git repo
|-- .pgpass         # Username/password file for local Postgres install
|-- .gitignore      # Define files (like .env) that won't be committed to git
|
|-- Procfile        # Specify what script is run on Heroku
|-- README.md       # Markdown documentation; formatted for github
|-- index.html      # Main page, with CSS/JS/img assets imported via link
|-- models         
|   |-- index.js    # Instantiate db object, connect to remote/local postgres
|   |-- order.js    # Mapping between Postgres table and fields of Order JS object
|-- package.json    # Define which npm modules are needed; used for Heroku deploy
|-- pgsetup.sh      # Set up local Postgres db from .pgpass for use by index.js
|-- setup-ssjs.sh   # Set up npm, heroku, and postgres for the app to run
|-- views          
|   `-- orders.ejs  # template for displaying Order instances as HTML
`-- web.js          # Main express app; defines /, /order, and /refresh_order routes
