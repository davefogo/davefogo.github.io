---
layout: post
title: blocmarks
thumbnail-path: "img/blocmarks.png"
short-description:   A bookmark management system that allows users to share their favorite sites while keeping them organized and easy to use.


---

{:.center}
![]({{ site.baseurl }}/img/blocmarks.png)

## Explanation

Along with the large amount of notes I had taken came the bookmarks where the information resided. I had too many bookmarks spread out in 2 different browsers. The bookmarks were so difficult to find that I had to look up bookmarked concepts again.

## Problem

The best way to solve my overcrowded bookmark situation was by creating blocmarks. blocmarks allowed me to stash bookmarks according to topics. An easy way to navigate and find what I needed to reference I a few clicks.

I was also aware that many users would carry in a large library of bookmarks. This is why I implemented a CSV uploader that allowed users to add the bookmarks they exported from browsers.

## Solution

A feature that blew my mind was the ability to send emails to blocmarks to create new bookmark entries in the database. All I had to do was implement and configure Mailgun to receive incoming emails. The email needs only the topic in the subject and the url in the body to be parsed and stored by blocmarks.

  >Liking bookmarks allowed users to remember which bookmarks owned by others they liked. The liked bookmarks would then be placed along with their own in their user profile for easy reference.


## Results

I have found blocmarks so useful that I have deployed it to heroku and use it on a daily basis. When I started the project I was concerned if blocmarks was going to be useable at completion. The large amount of bookmarks people had was going to be a barrier for adoption. The CSV uploader and saving bookmarks from received email neutralized this fear instantaneously.

## Conclusion

I will definitely keep email and database integration present for all of my future projects.
