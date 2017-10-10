---
layout: post
title: Bloc-It
thumbnail-path: ""
short-description: Bloc-It is an app to post, vote, share, and comment.

---

{:.center}
![]({{ site.baseurl }}/img/blocjams.png)

## Explanation

Bloc-It is an application similar to Reddit. Users can post, vote, share and comment on content. This applicaiton was built using Ruby.

## Problem

There were multiple different problems / objectives to this project:
- User must be able to manipulate posts and comments
- Posts were reconfigured by Topic
- Users were able to create an account and sign in / out
- User levels are created
- User can vote on a post and or favorite the post

## Solution

The first objective was to create a post. Using the MVC (Model, View, Controller) posts were created in the application. Based on that comments were created so that a user can comment on a post, each post having many comments. After seeding the database, rSpec testing was run to ensure that the application worked as expected. Then CRUD was applied, or the ability for a user to Create, Read, Update and Delete posts and comments.

An additional data object was added, Topics. Topics allowed for the reconfiguration of the posts to more easily find and or interact with posts that the user finds interesting. Each Topic having multiple posts. At this point the view was changed to view all of the topics, when a topic is clicked, all of the posts appear. Refactoring of the views was also necessary and partials added to keep the coding of this application efficient.

By using the Ruby Gem 'BCrypt', users were able to sign up and sign into and out of the application. At this point each user has their own posts and comments. 

Users were able to have different permissions in the application. Using :enum 3 roles were created. 1) Admin - Admin can create, update or delete any topic or post. 2) Member  - Members can create, update or delete their own posts. 3) Guest - Guests can only read posts in the application.

Users are also able to vote on posts and or comments. The application then shows the number of votes on that comment and gives the ability to vote up or down on the item. If the user really enjoys the item, they can favorite it. If a user favorites a post and there is a new comment, the user is emailed that there is a new comment on the post.  


## Results

The above resulted in a great Ruby application that allows user to interact with Posts similar to Reddit.

## Conclusion

The project was my first Ruby application. I learned about the relationships between objects and the flow of information around the application. As well as how each section relies on the other, this is also important in learning to route information so that there can be many files in an application so that it is easier to work on and troubleshoot.
