# Create an Node/Express app

- make a new directory--- mkdir [directory_name]
- cd into directory--- cd [directory_name] 
                -------In no specific order:------
- make an entry point file--- touch [file_name(usually index.js)]
- npm init -y (to say 'yes' to all the JSON questions)
- could add all the packages in one line--- npm i express ejs express-ejs-layouts Or        
separate lines: 
    - npm i express 
    - npm i ejs 
    -npm i express-ejs-layouts
- ignore all the node_module files --- echo "node_modules" >> .gitignore
- open VSCode--- code . 
                --------In VSCode--------
- in index.js file add lines below: 
                ----to incorparate the packages---
- const express = require('express')
- const app = express()
- const ejsLayouts = require('express-ejs-layouts') 
                ----for the middleware---
- app.set('view engine', 'ejs')
- app.use(ejsLayouts)
- add a views folder -add a home.ejs file -add a layout.ejs file
- add a controllers folder 
                ------get to working on the app----