---
layout: post
title: Bloc-Chat
short-description: Bloc-Chat is a user messaging system.

---

## Explanation

Bloc-Chat is a a real time chat application that allows for different users, chat rooms and messages. It is written using Angular, HTMl and CSS and stored in a Firebase Database for real time interaction.  

## Problem

There were multiple different problems to this project:
- View a list of chat rooms
- Create a new chat room
- View messages in each chat room
- Attach a username to each message
- Create a new message in the chat room with a username

## Solution

The first objective was to create a list of chat rooms. To do this a Firebase database was created and linked to the project. Then Angular was used to view all of the rooms in the Firebase database.

Then Bootstrap was used, specifically the $uibModal service to create a Modal to prompt for a new room and new room name. Using Angular added the new room to the application and the Firebase database.

Once the chat rooms were set, each message was to be viewed in the chat room. Using the $firebaseArray and creating a new message factory; each message in the chat room was able to be viewed.

To attached a username to each message, cookies were injected into the application. By using cookies the user was prompted to put in a username for that session that the browser was able to reference easily.

The last step was to create a new message. Once the new message was created, the username was associated with the message and sent back to the Database. The page would update with the new saved message.


## Results

The above steps resulted in a single page application that was user friendly and interactive. The user is able to sign in and go into multiple different chat rooms and chat in real time with other users.

## Conclusion

The project taught me a lot about coding using third party application. It was the first time using Firebase, and Bootstrap. It was very useful in an application like this to have a live database and a single page application. I believe that this significantly increases the user experience.
