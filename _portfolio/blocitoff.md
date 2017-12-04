---
layout: post
title: Bloc-Itoff
thumbnail-path: ""
short-description: Bloc-itoff is an app to create to do lists, which automatically deletes tasks that are over 7 days old.

---

{:.center}
![]({{ site.baseurl }})

## Explanation

Bloc-Itoff is an application where a user and sign in / out and create to do lists. Any item that is not checked off after 7 days is considered not important and automatically deleted.

## Problem

There were multiple different problems / objectives to this project:
- User must be able to sign in and out
- User can create multiple to do items and mark them complete  
- User can see how old the item is
- The application will automatically delete any to do item older than 7 days

## Solution

The first objective was to allow a user to sign in / out of the application. The Devise Gem was used to accomplish this.

Users can then create multiple to do items in the application. When the user signs into the application, they can view a list of their to do items. The next step was to create the destroy function, this allows users to mark their items complete and the to do item to no longer appear.

Using the distance_of_time_in_words helper method, the time since the item was created was shown to the user. The last item was to use the Rake utility to delete any task that was older than 7 days.

## Results

The above resulted in a great Ruby application that allows user to create and mark off to do list items.

## Conclusion

The project was great to independently create items and delete items per the user. It taught me about utilities so that applications can have more functionality to automatically go through and adjust databases.
