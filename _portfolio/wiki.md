---
layout: post
title: Bloc-Wiki
thumbnail-path: ""
short-description: Bloc-Wiki is an application to have users collaborate on content.

---

{:.center}
![]({{ site.baseurl }})

## Explanation

Bloc-It is an application similar to Wikipedia where users can sign in and create Wikis. Then collaborate information with the application community.

## Problem

There were multiple different problems to this project:
- User must be able to sign up for an account
- Users can create, read, update and delete wiki's
- Users can have accounts at 3 membership levels
- Users can upgrade account to a paid subscription
- Users can add / remove collaborators to their wiki's

## Solution

The first objective was to allow a user to sign into the application. The Devise gem was installed and set up for this use.

A wiki model/controller/view was created.  After seeding the database using the gem Faker, rSpec testing was run to ensure that the application worked as expected. Then CRUD was applied, or the ability for a user to Create, Read, Update and Delete their wiki's.

Users were able to have different permissions in the application. Using the Pundit gem for authorization 3 roles were created. 1) Standard (free) - Standard users can create, update or delete their wiki's. 2) Premium  - Premium members have a paid subscription and can Members can create, update or delete their own wikis, as well as make them private. The upgrade was implemented using Stripe integrations. 3) Admin - Admin users can create, edit, and delete any wiki.

Users are also able add and remove collaborators to their wikis. This helps in the exchange of ideas and information across platforms. Each wiki can have many collaborators and each user can be a collaborator on many wikis.


## Results

The above resulted in a great Ruby application that allows user to interact with wikis and exchnage information similar to Wikipedia.

## Conclusion

This project allowed me to rely on Gems and how they can be used to create an application. This helps to install a Gem and learn how they interact with the application instead of writting each line of code out to accomplish the same task. It was also interesting to plug into Stripe Api to be able to charge for subscriptions and to see how that interaction worked. 
