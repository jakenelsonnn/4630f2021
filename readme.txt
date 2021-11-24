Name: Jacob A. Nelson
Course: Mobile Application Development 1
University: Umass Lowell
Semester: Fall 2021

Project Name: Poll App (tentative title - will come up with a better one soon!)

Sections of this README
1. Project Proposal Form
2. Weekly Progress Reports

*********************************************************************

SECTION 1: PROJECT PROPOSAL FORM
These are questions from the project proposal and my answers to them.

What is the problem you aim to tackle with your project?

People of all backgrounds and professions need an easy-to-use and dedicated platform to conduct and respond to
polls. There are ways of polling digitally, like social media, but not everyone uses social media, and the polls
a user can conduct on Facebook or Twitter are somewhat limited. The app I aim to develop over the course of 
this semester (perhaps over another semester, as well) will be an app where people can respond to and conduct 
polls.


Why is this problem important to tackle?

Polls are an essential way of gathering all sorts of data. They can be time consuming to conduct, and this app
would take away the hassle and make gathering data from people a very easy task.


Who stands to benefit from this app most? (I.e., who is your expected "market")

Everyone, because that who uses polls. This app could particularly give a hand to people conducting market 
research, as creating surveys is a large part of the field. It could also be used by team leaders, hoping to
easily democratize a decision-making process with a large team of people. It could also be used by teachers
who wish to conduct polls (or even quizzes!) for their students.


List other apps that have addressed the same problem.

Pollie


For the app you listed above, list in what ways it is lacking.

There are a lot of apps that are exactly similar to Pollie, so I did not bother to include them. The biggest
flaw that Pollie and its likenesses have is how they limit polls to consist of just one question.


For each shortcoming you have identified above, state whether you intend to address it, and how.

The app I will develop will allow a poll to consist of multiple questions in one place. This might seem like
a nitpick, but it many surveys or polls consist of multiple questions. With Pollie, a user would have to create
several polls and send those multiple polls to people they want answers from, which is a pain.


Your "elevator pitch."

People need an easy-to-use and dedicated platform to conduct and respond to polls. In this app, people can create
their own polls with as many questions and responses to each question that they might desire. This app will be
distinct from others like it because of its flexibility. Other poll apps do not typically allow users to have polls
that have multiple questions, but this app will. Further down the road, this app will have even greater flexibility,
as I will add features such as allowing users to create various types of questions, such as answering questions with
a sliding scale (0 to 100, for example) and the ability to view the results graphically, such as with a pie chart
or bar graph, depending on the data.


List any technologies you are considering for your project.

Android Studio with XML and Java. I am planning on using Android's Room API to assist in the SQL/database aspect
of the program, like saving/retrieving login information and data about polls.

*********************************************************************

SECTION 2: WEEKLY PROGRESS REPORTS

In this section I will roughly recap the progress I have made on this project each week. I may discuss things I
have added, things I plan on adding, and things I have learned during the week, such as android development topics
that may or may not have been implemented into the app at the time.

WEEK ONE: (SUBMISSION DATE: NOV. 3)

App Progress:
-created login and signup activities and designed their layout. Login/Signup implementation will be added later.
-implemented navigation between the two activities: can click "sign up" on login page to be brought to the signup
page. At this time both pages have EditTexts for email and password. A user can enter text into them, but they
currently do not do anything.

Learned (or learning) this week:
-Android Room API: a library in Java that encapsulates a lot of SQL database managment functions. I will need
this library when I implement both the login/signup features and the poll features.
-RecyclerView: A view container that is adaptive to new things being put into it during the application/activity
lifecycle. I will need this sort of container for various parts of my app in the near future.

--------------------------------

WEEK TWO: (SUBMISSION DATE: NOV. 10)

App Progress:
-created/started "Home" activity, where user can see a list of their currently active polls.This activity features
a side navigation bar, which contains the following options for the user: "My Polls," "Find Poll," and "Log Out."
These options currently do not do anything when clicked at this time but in the future they will open the appro-
priate activity when they are selected. The side menu bar has a header, which shows the user's email that
is associated with the account and their name (sampleText for now). It also has a placeholder for some sort of
image next to the name and e-mail, which I think I will make a sort of "profile picture" for the user. An idea
I have for a default profile picture for a user is just an image with the first letter of their name in it (like
Google's default profile picture for users).
-The user can navigate to the Home page by pressing the "login" button from the main activity, or the "signup"
button from the signup activity.

TODO/future plans
-This activity is of course not complete, but for now I have filled the body of the page with sampleText text views.
This is where the titles of the user's currently active polls will go. The user will be able to click on them and
be brought to a page containing info about that particular poll.
-I will also add a floating activity button with a '+' image in it which will be the "add poll" button.
-The poll list itself will not consist of text views, but with custom views, which will be nice "container" views
for the polls which will show not only the title of the poll but the start date and end date, number of responses,
and number of questions.


--------------------------------

WEEK THREE (SUBMISSION DATE: NOV 17)

App Progress
-created working login and signup modules for my signup/login activities. Now a PollApp user can actually create
an account and use it to login to the app on future returns. This information is stored in a local database on
the device. At this time all databases that this app will use (during its current state of development) will all
be stored locally. In the future, I will learn about cloud-based database services, but at this current time, I
don't know enough about that subject to incorporate it into my project.

The database is created using Android's Room API, which allow you to code objects to represent various components
of MySQL database features. This was an incredibly helpful API because it allowed me to create and use a MySQL
database for my app without having to know a huge amount about MySQL. It really works, too. You can create an
"account" on pollApp and it will save the information the user gave it to log in to the app at a later time. It
features input validation from the user, making sure they input all fields, and that their password confirmation
matches, and making sure they are registered in the system. A successful login will bring the user to the home
activity.

TODO/future plans
-Start building other fragments and activities for the rest of the app. This upcoming week I plan on designing
the activities/fragments for "Find Poll" and "Create Poll" and make sure the design works properly before adding
the back-end features to it. After that, I am going to have to figure out a way to represent polls as MySQL enti-
ties. That part is going to be a big obstacle because due to the nature of the app, the options for polls will be
robust in terms of how many questions or what type of questions they may contain, so designing the entities for
polls will be a challenge I need to spend some time on. 

--------------------------------

WEEK FOUR (SUBMISSION DATE: NOV 24)

App Progress:
Developed the home screen: implemented a RecyclerView to hold custom CardViews that will be linked to polls. The
home screen is filled with sample polls at this time rather than just sample text. Also implemented navigation
in the Home activity, so the "Add poll" and "Find poll" features will be fragments within the activity. At this
time the fragments for "Add poll" and "Find poll" are blank.

Also made it so it displays the email/username in the navigation header.

TODO/Future plans
Start designing the "Find Poll" and "Create Poll" fragments. The "Create Poll" aspect will involve allowing the
user to design polls with as many questions as they would like, so I will need to implement something like a
RecyclerView in which additional questions (and possible answers to those questions) can be added to the Recycler-
View.
