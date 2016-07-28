*Summary*
  The summary of a case study should be short and to the point. It should define the basics of the project you've worked on. A brief sentence or two should suffice, focusing on the problem or outcome of the project.
*Explanation*
  The explanation of a case study will describe the backstory of the project, the key players (featuring both users and stakeholders), your relationship with the project, and what roles you played.
*Problem*
  The problem is what you were hired to solve. This usually lists the reasons why you were brought on board and the issues you were given to resolve. Once you establish the list of problems, you can further expand on each and how they relate to the project you're working on.
*Solution*
  You should discuss your solutions and back your decisions up with conducted research. You can explain the solution to each problem separately. Provide reasoning that supports the fixes you proposed. You should also display screenshots or artifacts of your presented solutions. Include all assets created in the design or development process. Explain your work and the theory behind it.
*Results*
  Testing is a big part of the design and development process. Understanding whether or not your solutions worked is essential. Provide information about your testing process then share the results you discovered from your users.
*Conclusion*
  After sharing your solutions, you should summarize your final thoughts on the project. Ask yourself the following:

  What worked?
  What didn't?
  What were your doubts going into the project?
  What surprised you the most?
  What would you have done differently?
  What did you learn while doing this project?
  How will you use that information in the future?




**ideapp**
Summary:
  ideapp is an Enterprise Resource Planning software based on Ruby on Rails designed specifically for ideamos, an Advertising Agency in Bogota, Colombia. This is the first programming I ever did.

Explanation:
 A side project that came to existence to solve a problem for ideamos, the company I work for. ideamos operates in the advertising industry in Colombia. As a Finance Director there, I could not find a suitable ERP to run the company's Finance department.

Problem:
 I found myself using excel spreadsheets to calculate numbers and a "software solution" to feed the data. The company's other areas were operating using a similar technological approach. After demoing various "industry specific" solutions I came to the conclusion that there was simply no good software available for ideamos to use.

Solution:
  After the realization, I began the quest to build ideapp via trial/error (no testing suite used), copy/pasting from tutorials and a lot of searching in stackoverflow. I had to use Devise and Pundit (after I realized that Can Can was no longer maintained) to make sure only users from one department had access to what their roles permitted them to.

Results:
  At this moment ideapp is in its alpha version. It has undergone various successful production tests in the Finance and Media Purchasing departments. To deploy the ERP in production, the code must be adjusted to meet Colombia's government new financial reporting standards.

Conclusion:
  This project took most of my free time away but it was a lot of fun to experiment and create.

**bloccit**

Summary
  A reddit clone that introduced the basics of Ruby on Rails.

Explanation
  This application allowed users to create posts, comment on them, save them as favorites and even vote them up or down. Unlike the very first project I did, this one uses standard testing.

Problem
  The main feature for bloccit was to be able to keep tabs on what posts and comments a user had written. This feature was centralized in the user's profile allowing a simple and fast way to access their content.

Solution
  Signing up was solved using a custom made authentication and authorization solution. This allowed me to understand the power of restricting access using rails' controllers.

  Commenting, up-voting or down-voting posts was made magical with ajax and its non-obtrusive JS. This really amazed me!

  Test-Driven-Development (wish I had used this in my first project) was the greatest tool to assure assertive and simple code.

  Building an API taught me the now industry standard way of how developers interact with developers.

Results
  The intended features worked as expected.

Conclusion
  The large amount of intermediate and advanced material I learned with this project will serve as a launching pad for my next creations.

**alexa-lego-trivia**

Summary
  The creation of an Amazon Alexa skill opened my eyes to the immense possibilities available through AI.
  This app is a game that enables owners of Alexa ready devises to navigate vocally in a fun trivia game about all things LEGO.      

Explanation
  Before I started this project I was always curious to understand how AI worked. Developing for the Amazon Alexa team was a great way to start in the field. The main core of my Alexa Skill is developed using Javascript and node.js. Amazon's developing suite allowed me to learn how apps are hosted using Amazon Web Services.

Problem
  The goal for this project was to learn the development of Alexa Skills. Users who used the app would need to use specific "intents" to begin the game. To cover the greatest number of users it was crucial to come up with a large variety of "intents".

Solution
  I looked at other Alexa skills and used LEGO specific language as reference to create the intents.

Results
  Trivia Game for LEGO was certified and published by Amazon on July 21st, 2016. When I completed the project I wanted to keep adding trivia questions to my skill, thus it is still a work in progress.

Conclusion
  Alexa skills and enabled devices have grown substantially in the past 8 months. The ease of use of Alexa will secure the success of the technology. This leads me to think that any successful company, will need to develop their own Alexa Skill to complement any technology available to their customers.

**blocipedia**

Summary
  An application based on the idea of creating content and sharing it with others. Allowed me to dwell deeper into the understanding of Ruby on Rails.

Explanation
  The reason I started this project was to tackle a problem of my own. Since I started learning to program I had accumulated vast amounts of information. I needed to consolidate all the information  scattered in notebooks and text editors. From the planning stage to the completion of the project I was    focused on the ease of use. I wanted blocipedia to feel familiar to its users while allowing crucial features to flourish.
Problem
  In this project I integrated the Stripe payment solution to allow users to upgrade their standard membership to premium by paying a fee. Premium users had the ability to create private "wikis", pages that are exclusive for them to view and edit.
Solution
  Collaboration was a key feature when users wanted to share the authorship of an article with others. By using the "Has Many Through" relationship I enabled users to invite various other members to edit their "wikis". Any given user could be a collaborator in one or more "wikis".
Results
  Although blocipedia has many valuable features, it proved to be incredibly hard to adopt. At least for users with a lot of handwritten notes, it would be costly to type the information into blocipedia.
Conclusion
  This project used custom made user authentication and authorization. If I had to develop this project    again from scratch I would implement this feature using Devise and Pundit for the sake of maintainability. It would be much easier for a developer to change roles and modify specific needs using industry standard technology.

**blocmarks**

Summary
  A bookmark management system that allows users to share their favorite sites while keeping them organized and easy to use.

Explanation
  Along with the large amount of notes I had taken came the bookmarks where the information resided. I had too many bookmarks spread out in 2 different browsers. The bookmarks were so difficult to find that I had to look up bookmarked concepts again.
Problem
  The best way to solve my overcrowded bookmark situation was by creating blocmarks. Blocmarks allowed me to stash bookmarks according to topics. An easy way to navigate and find what I needed to reference I a few clicks.

  I was also aware that many users would carry in a large library of bookmarks. This is why I implemented a csv uploader that allowed users to add the bookmarks they exported from browsers.

Solution
  A feature that blew my mind was the ability to send emails to blocmarks to create new bookmark entries in the database. All I had to do was implement and configure Mailgun to receive incoming emails. The email needs only the topic in the subject and the url in the body to be parsed and stored by blocmarks.

  Liking bookmarks allowed users to remember which bookmarks owned by others they liked. The liked bookmarks would then be placed along with their own in their user profile for easy reference.

Results
  I have found blocmarks so useful that I have deployed it to heroku and use it on a daily basis. When I started the project I was concerned if blocmarks was going to be useable at completion. The large amount of bookmarks people had was going to be a barrier for adoption. The csv uploader and saving bookmarks from received email neutralized this fear instantaneously.

Conclusion
  I will definitely keep email and database integration present for all of my future projects.
