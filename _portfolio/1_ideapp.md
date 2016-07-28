---
layout: post
title: ideapp
thumbnail-path: "img/ideapp.png"
short-description: ideapp is an Enterprise Resource Planning software based on Ruby on Rails designed specifically for ideamos, an Advertising Agency in Bogota, Colombia. This is the first programming I ever did.

---

{:.center}
![]({{ site.baseurl }}/img/ideapp.png)

## Explanation

A side project that came to existence to solve a problem for ideamos, the company I work for. ideamos operates in the advertising industry in Colombia. As a Finance Director there, I could not find a suitable ERP to run the company's Finance department.

## Problem

I found myself using excel spreadsheets to calculate numbers and a "software solution" to feed the data. The company's other areas were operating using a similar technological approach. After demoing various "industry specific" solutions I came to the conclusion that there was simply no good software available for ideamos to use.

## Solution

After the realization, I began the quest to build ideapp via trial/error (no testing suite used), copy/pasting from tutorials and a lot of searching in stackoverflow. I had to use Devise and Pundit (after I realized that Can Can was no longer maintained) to make sure only users from one department had access to what their roles permitted them to.

## Results

At this moment ideapp is in its alpha version. It has undergone various successful production tests in the Finance and Media Purchasing departments. To deploy the ERP in production, the code must be adjusted to meet Colombia's government new financial reporting standards.

## Conclusion

This project took most of my free time away but it was a lot of fun to experiment and create.
