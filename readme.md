# Add Mongoose
* Install and configure Mongoose
* Setup campground model
* Use campground model inside of our routes

# Show Page
* Review the RESTful routes we've seen so far
* Add description to our campground model
* Show db.collection.drop()
* Add a show route/template

# Refactor Mongoose Code
* Create a models directory
* Use module.exports
* Require everything correctly!

# Add seeds file
* Add a seeds.js file
* Run the seeds file every time the server starts

# Add the Comment model
* Make our errors go away!
* Display comments on campground show page

# Comment New/Create
* Discuss nested routes
* Add the comment new and create routes
* Add the new comment form

INDEX   /campgrounds
NEW     /campgrounds/new
CREATE  /campgrounds
SHOW    /campgrounds/:id

NEW     campgrounds/:id/comments/new    GET
CREATE  campgrounds/:id/comments        POST

## Style Show Page
* Add sidebar to show page
* Display comments nicely

## Finish Styling Show Page
* Add public directory
* Add custom stylesheet

## Auth Pt. 1 - Add User Model
* Install all packets needed for auth
* Define User model

## Auth Pt. 2 - Register
* Configure Passport
* Add register routes
* Add register template

## Auth Pt. 3 - Login
* Add login routes
* Add login template

## Auth Pt. 4 - Logout/Navbar
* Add logout route
* Prevent user from adding a comment if not signed in
* Add links to navbar
* Show/hide auth links correctly

## Auth Pt. 5 - Show/Hide Links
* Show/hide auth links in navbar correctly (login and sign up or logout if logged in) 

## Refactor The ROutes
* Use Express router to reorganize all routes

## Users + Comments
* Associate users and comments
* Save author's name to a comment automatically

## Users + Campgrounds
* Prevent an unauthenticated user from creating a campground
* Save username+id to newly created campground

# Editing Campgrounds
* Add Method-Override 
* Add Edit Route for Campgrounds 
* Add Link to Edit Page 
* Add Update Route 

# Deleting Campgrounds 
* Add Destroy Route 
* Add Delete Button 

# Authorization 
* User can only edit his campgrounds 
* User can only delete his campgrounds 
* Hide/Show edit and delete buttons 

# Refactoring Middleware 

Campground Edit Route: <!-- /camgrounds/:id/edit -->
Comment Edit Route: <!-- /campgrounds/:id/:comment_id/edit -->

# Deleting Comments
* Add Destroy route
* Add Delete button
* Add update route

Campground Destroy Route: <!-- /camgrounds/:id -->
Comment Destroy Route: <!-- /campgrounds/:id/comments/:comment_id -->

# Authorization Part 2: Comments
* User can only edit his comments
* User can only delete his comments
* Hide/Show edit and delete buttons
* Refactor Middleware

# Adding in Flash!
* Demo working version
* Install and configure connect-flash
* Add bootstrap alerts to header

# Git - git-scm.com

## Introduction
* What is Git? Is a version control system, it's a technology
* What is Github? Is an application, a web site, that works with Git
* Git x Github - are not the same!
* Installing Git

# Git Basics
* Git init
* Git add
* Git commit

# Git checkout
* Git log
* Git Checkout

# Cloning and Github Intro
* Creating a repo on a github
* Adding a remote
* Pushing to Github

============================

# Git - git-scm.com

## Introduction
* What is Git? Is a version control system, it's a technology
* What is Github? Is an application, a web site, that works with Git
* Git x Github - are not the same!
* Installing Git

# Git Basics
* Git init - usually at the project folder
* Git status 
* Git add
* Git commit 

# Git checkout - to get back to previous versions
* Git log - shows all the commits I've made / press Q to quit
* Git Checkout - copy and paste the id from the commit I want to check / to go back to the master = git checkout master
* git revert --no-commit XXXXX..HEAD

# Cloning and Github Intro
* Creating a repo on a github
* Adding a remote
* Pushing to Github

=====================================================
ANOTAR NO MEU ARQUIVO WORD - WINDOWS!!!

video GIT Colt
https://www.youtube.com/watch?v=USjZcfj8yxE

VIDEOS IAN git
https://www.youtube.com/watch?v=LemSseuZB9I&list=PL86ehqHzxhy4XX_qZZE_5mrp38WGZRzTO

link GIT tutorial
https://www.notion.so/Introduction-to-Git-ac396a0697704709a12b6a0e545db049#d5e9c2b6379246a593c1ef74051e7e3c

YELPCAMP avancado
https://github.com/nax3t/yelp-camp-refactored
=======================================================

git commit -m "MINHA MENSAGEM NO PRESENTE"


=============
# DEPLOYING

## GIT
* git init (na pasta principal do projeto)
* git status
* git add nomeDoArquivo / ou / git add . ("." ponto adiciona todos os arquivos)
* git commit -m "minha mensagem"

## HEROKU
* heroku login -i
* heroku create
* no arquivo 'package.json' escrever: "start": "node app.js" - após "test" (ultima propriedade (item) do primeiro objeto)
* git push heroku master

# APOS MODIFICAR ARQUIVOS
* se eu modificar algum arquivo, preciso repetir:
* git status - para ver o que foi modificado, etc
* git add nomeDoArquivo
* git commit -m "minha mensagem"
* git push heroku master

# ERROS
* heroku logs

# heroku run +comando (usado na linha de comando)
* heroku run ls - para ver os arquivos e pastas no heroku
heroku run ls node_modules - para ver quais node modules foram instalados
* heroku run npm install mongoose --save, etc...
