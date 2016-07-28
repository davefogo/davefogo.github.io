---
layout: post
title: blocipedia
thumbnail-path: "img/blocipedia.png"
short-description: A production quality application based on the idea of creating content and sharing it with others. Allowed me to dwell deeper into the understanding of Ruby on Rails.

---

{:.center}
![]({{ site.baseurl }}/img/blocipedia.png)

## Explanation

The reason I started this project was to tackle a problem of my own. Since I started learning to program I had accumulated vast amounts of information. I needed to consolidate all the information  scattered in notebooks and text editors. From the planning stage to the completion of the project I was    focused on the ease of use. I wanted blocipedia to feel familiar to its users while allowing crucial features to flourish.

## Problem

In this project I integrated the Stripe payment solution to allow users to upgrade their standard membership to premium by paying a fee. Premium users had the ability to create private "wikis", pages that are exclusive for them to view and edit.

## Solution

Collaboration was a key feature when users wanted to share the authorship of an article with others. By using the "Has Many Through" relationship I enabled users to invite various other members to edit their "wikis". Any given user could be a collaborator in one or more "wikis".

## Results

Although blocipedia has many valuable features, it proved to be incredibly hard to adopt. At least for users with a lot of handwritten notes, it would be costly to type the information into blocipedia.

## Conclusion

This project used custom made user authentication and authorization. If I had to develop this project    again from scratch I would implement this feature using Devise and Pundit for the sake of maintainability. It would be much easier for a developer to change roles and modify specific needs using industry standard technology.
