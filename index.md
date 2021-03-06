<img src="doc/StudBudd3-transperent.png">

# Development Progress 
- [Our current StudBudd Web App](http://studbudd.meteorapp.com/#/)
- [Milestone 1](https://github.com/studbudd/studbudd/projects/1) 
- [Milestone 2](https://github.com/studbudd/studbudd/projects/2) 
- [Milestone 3](https://github.com/studbudd/studbudd/projects/3) 


# StudBudd Goals

Our goal for StudBudd is to create a Meteor application to provide the students of  the University of Hawaii with an opportunity to list courses they have taken for which they are willing to attempt to provide help. Also courses they are currently taking for which they might need help in.

# User Guide

When you first visit the page, you will be greeted by our Landing Page!
<img src="doc/MS3-LP.png">

Anyone from the UHM or even outside of the university can create an account to search for help.

<img src="doc/MS3-SIGNUP.png">

Once you are signed in, you can visit the Classes page. You will be greeted by an empty page with a list of classes on the left. Clicking on a class will display a list of mentors that are proficient in that class.

<img src="doc/MS3-CLASS.png">

You can also visit the mentors page, in which you will be greeted with a full list of all of the available mentors and the subjects they are offering mentoring in. 

<img src="doc/MS3-MENTOR.png">

If you are logged in as a mentor or student, Visiting the students page will display all the students and the subjects they are looking for help in. When a student is clicked, you will be redirected to their profile. From there, as a mentor you can offer help. As a student, you can plan group study sessions that student if you need help in the same subject.

<img src="doc/MS3-STUDENT.png">

# Community Feedback
UH alumni,Brandon Chun, said to change the title for visibility and edit the mentor card so the so information is more clear, and to range our pages. He also was not thrilled with the name 'StudBudd' and recommended 'StudMuffin'. Other comments,from another former UH student, focused on the aesthetics of the cite, and a few concerns about functionality. 

"The pages that have a darker background are easier on the eye but the landing page picture could be better." - Sean Brown, UH alumni 

"It looks like a great way to connect with peers and get help with classes that may be particularly tough." -Kahlin, UH student 

"Neat and organized, but the heading is a little hard to read." -Kailey, UH student 




# Development history
- Milestone 1
+ Landing page
+ Mockup pages for classes, tutors, and admin functions
<img class="ui small right floated rounded image" src="doc/landingpage.png">

- Milestone 2
+ Mentor and student collections
+ Added functionallity to mockup pages: tutors, classes, and student listings
<img class="ui small rounded image" src="doc/LPupdated.png"><img class="ui small rounded image" src="doc/registerPage.png"><img class="ui small rounded image" src="doc/classesAvailable.png"><img class="ui small rounded image" src="doc/tutorsAvailable.png"><img class="ui small rounded image" src="doc/studentsList.png">

- Milestone 3
+ Added Calendar function
+ Added Edit function to mentor, student and calendars
+ Added filter function to classes page 
+ Improve asthetics

# Developer Installation Guide

First, [install Meteor](https://www.meteor.com/install).

Second, [create a new GitHub repository](https://help.github.com/articles/create-a-repo/), and clone it into your local workspace.

Third, [download a zip file containing a snapshot of meteor-application-template-react](https://github.com/ics-software-engineering/meteor-application-template-react/archive/master.zip).

Fourth, uncompress the zip file, and copy the following files and directories into your repo:

  * app/  
  * config/
  * .gitignore
  
You don't need to copy the README.md or index.md files (you should write your own), and you don't need to copy the doc/ directory (it contains only screenshots displayed in this page of documentation.)

Now your local repo should contain the template. To test that everything is OK, cd into the app directory install the required libraries with:


```
$ meteor npm install
```

Once the libraries are installed, you can run the application by invoking the ["start" script in the package.json file](https://github.com/ics-software-engineering/meteor-application-template-react/blob/master/app/package.json):

```
$ meteor npm run start
```

The first time you run the app, it will create some default users and data. Here is the output:

```
meteor npm run start

> meteor-application-template-react@ start /Users/philipjohnson/github/ics-software-engineering/meteor-application-template-react/app
> meteor --no-release-check --settings ../config/settings.development.json

[[[[[ ~/github/ics-software-engineering/meteor-application-template-react/app ]]]]]

=> Started proxy.                             
=> Started MongoDB.                           
I20180227-13:33:02.716(-10)? Creating the default user(s)
I20180227-13:33:02.742(-10)?   Creating user admin@foo.com.
I20180227-13:33:02.743(-10)?   Creating user john@foo.com.
I20180227-13:33:02.743(-10)? Creating default data.
I20180227-13:33:02.743(-10)?   Adding: Basket (john@foo.com)
I20180227-13:33:02.743(-10)?   Adding: Bicycle (john@foo.com)
I20180227-13:33:02.743(-10)?   Adding: Banana (admin@foo.com)
I20180227-13:33:02.744(-10)?   Adding: Boogie Board (admin@foo.com)
=> Started your app.

=> App running at: http://localhost:3000/
```


**Note regarding bcrypt warning.** You will also get the following message when you run this application:

```
Note: you are using a pure-JavaScript implementation of bcrypt.
While this implementation will work correctly, it is known to be
approximately three times slower than the native implementation.
In order to use the native implementation instead, run

  meteor npm install --save bcrypt

in the root directory of your application.
```

On some operating systems (particularly Windows), installing bcrypt is much more difficult than implied by the above message. Bcrypt is only used in Meteor for password checking, so the performance implications are negligible until your site has very high traffic. You can safely ignore this warning without any problems during initial stages of development.

If all goes well, the template application will appear at [http://localhost:3000](http://localhost:3000).  You can login using the credentials in [settings.development.json](https://github.com/ics-software-engineering/meteor-application-template-react/blob/master/config/settings.development.json), or else register a new account.

Lastly, you can run ESLint over the code in the imports/ directory with:

```
meteor npm run lint
```

# Page Modeling

This page is what we'll be modeling

<img src="doc/template.png">

