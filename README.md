# Pethero

## Overview
Are you tired of losing your pets and relying on outdated paper flyers to reunite you with your beloved animal? Look no further, Pethero is here to save the day. Pethero is an online platform where users can make posts about pets they have lost or pets they have found. If a User finds a lost pet, they can confirm on Pethero if the distinct feature that the pet owner submitted matches what we have in our database. If that infomation is correct, the lost pet status changes from lost to waiting and the pet owner is notified via email that their pet may have been found. 

![ScreenShot](static/images/pet_show_page.PNG)

## Technologies Used 

 ### Languages
- Python 
- Javascipt 
- HTML
- CSS


 ### Frameworks
 - Flask
 - Bootstrap 
 - Semantic UI
 
## Installation Steps 

### Virtual Env
```
git clone https://github.com/lfonzi62/Project-4.git
cd Project-4 
```

```
$ pip3 install virtualenv
$ virtualenv .env -p python3
$ source .env/bin/activate
```
### Dependencies
``` 
bcrypt
flask
flask-bcrypt
flask-login
flask-wtf
itsdangerous
peewee
wtforms
``` 
```
$ pip3 install flask flask-login flask-bcrypt peewee flask-wtf itsdangerous wtforms
$ pip3 freeze > requirements.txt
```
### The App
You will need to create a secret.py that contains the following variables 
```
EMAIL_PASSWORD = "password for the email below "
SENDER_EMAIL = "email that you want to send to users after registration and finding pet"

URL_SAFE_SECRET = "secret key for token serializer"

APP_SECRET_KEY = "Secret key for your app"
```
### User Stories
- A user must register for an account
- A user must validate their email
- A user can sign in to view the different categories of pets
- A user can create a post about a lost pet or found pet 
- A user can edit and delete their pets information 
- A user can confirm if they found other user's pet 
- A user can leave comments about a pet
- Users can use the live chat feature to communicate with other users who are signed into the app
- Also found here while publically available https://trello.com/b/5mWq9FNR/petfinder


## Entity Relationship Diagrams

![ScreenShot](static/images/ERD_Project4.jpg)

## Planned Features
- Calendar system that allows user to schedule meetups for found pets 
- Upvote/downvote for comments
- Deployment on Heroku 
- Private messsaging option between users 
- Intergrate recursive comments
