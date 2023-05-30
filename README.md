# Specification
Chat - Chat - an application that allows us to communicate between 2 computers online.<br>
The application consists of 2 modules (server part and user part).<br>
The server part is made in the php Yii2 framework and the user part in the WPF framework, application uses rest Api.<br>
[Wpf repo](https://github.com/novy213/chat-user) <br>
[Server repo](https://github.com/novy213/chat-server) <br>
## Data range:
User: each user will have the following fields:<br>
- id
- login
- password
- name
- last name

Chat: each project will consist of the following data:
- id
- message
- user_from
- user_to

## Functions:
1. Login/Registration
2. Writing a message

## Database specification
The database contains 3 tables properly connected with each other.
### Users table:
- id - unique user ID
- login - user login
- password - user's encrypted password
- name - user's name
- last name - user's last name
- token - random 32 length text that is our authorization key
### Projects table:
- id - unique id of the project
- message - the field where is message
- user_from - unique id of user that send message
- user_to - unique id od recipient of the message
# Installation
