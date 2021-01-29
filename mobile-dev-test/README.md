# Overview

This is a coding exercise to help us assess candidates looking to join one of our mobile (iOS or Android) teams at Condé Nast. 

The task is intended to be completed at home. We appreciate the time you spend on it and we will go through your submitted work together when you're invited for the technical interview.

# Interview Resources

## Briefing

Build an application that shows the latest news from the United States, using the [newsapi.org](https://newsapi.org) service.

Running the app we should be able to see a list with the latest **US top headlines news** (see [newsapi.org documentation](https://newsapi.org/docs/)).
Each news item in the list should have the description of the article, the author, and the image associated to it. 
If the news doesn't have an image, present an image placeholder of your choice.

If the user clicks on a news item it will navigate to a new screen displaying the full news article selected, and some info regarding it.

The additional info are the number of **likes** and the number of **comments** the news item has.
That information can be retrieved from two internal not authenticated endpoints: 

 * `https://cn-news-info-api.herokuapp.com/likes/<ARTICLEID>` 
 * `https://cn-news-info-api.herokuapp.com/comments/<ARTICLEID>`

 The  `<ARTICLEID>`  is the article URL without the scheme and with the `/` replaced with a `-`.
For the article `https://www.theverge.com/2020/7/21/21332300/nikon-z5-full-frame-mirrorless-camera-price-release-date-specs/index.html` the `ARTICLEID` is `www.theverge.com-2020-7-21-21332300-nikon-z5-full-frame-mirrorless-camera-price-release-date-specs-index.html`

The app should have tests around the functionalities.
Although UI and UX are important, the goal of this demo is to show your thought process and how you architect your application. The design should take into consideration features that might be added in the future, like for example, offline reading, bookmarking, audio etc.

## Assessment Criteria

These points serve as a guide on what we look for in a code submission. Not all points have to be met:
 - The solution fulfils the brief
 - There is a README that instructs how to run the app
 - There is some attempt at creating documentation
 - The app runs when you follow the README or run the app
 - There are reasonably thorough tests (We consider tests to be as important as functional code)
 - The file/folder structure is intuitive
 - Code style is consistent
 - Chosen technologies are appropriate
 - Complex sections of code are readable/commented/justified
 - Not over-simplified or over-engineered

Please be prepared to have a discussion around the architectural decisions or any other questions we might have for the solution provided.

## Submission Information

We prefer to see your work as a GIT repo with commits from which the app is built up.
You can submit by sending up the link to a public git repository on Github, or if you'd 
like to keep the submission only between us, use [git bundle](https://git-scm.com/docs/git-bundle) and submit the zipped work.

Send the work to your **point of contact**.

## FAQ

Q: **Should I commit my `newsapi.org` token?**  
A: No, but please provide one for us

Q: **What version of iOS/Android must I support?**  
A: For testing purposes you can use the latest versions for Android and iOS but be prepared to have a discussions around what changes might be required if we did support older versions

Q: **Can I use libraries, frameworks, CocoaPods etc?**  
A: Yes, but be prepared to justify why you did so.
