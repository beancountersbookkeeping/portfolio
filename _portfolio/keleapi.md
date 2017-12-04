---
layout: post
title: Kele-Api
thumbnail-path: ""
short-description: Kele-Api was cerated to access the student endpoints of Bloc.
---

{:.center}
![]({{ site.baseurl }})

## Explanation

Kele-Api is an Api created to access the student endpoints of the Bloc school.

## Problem

There were multiple different problems / objectives to this project:
- Initialize and authorize Kele with a Bloc username and password
- Retrieve the current user as a JSON blob, mentor availability, roadmaps and checkpoints
- Interact with messaging function of Bloc
- Submit checkpoint assignments

## Solution

To start a RubyGem shell was created and httpart was installed. This allowed the Api to interface with HTTP requests. The first being, the Bloc sessions username and password to allow for sign in / out of the system.

Using authorization tokens against the Bloc Api information was able to be read between the Kele Api and Bloc Api. This was tested using the irb (interactive ruby shell).

Using the functions created in the Kele lib; not only read the information from Bloc, but enter information into the Bloc system. This allowed for messages and checkpoint submissions to be saved in the Bloc school database.


## Results

The above resulted in a great Kele Api that interacted with the Bloc school Api.

## Conclusion

The project was my first RubyGem. I learned about the endpoints of an Api and how to plug an Api or application into an existing Api that you didn't create. It was challenging to not only read information from the Bloc school system but to push information into the database.
