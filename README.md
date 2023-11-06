# README
Unfortunately, due to time limit on demo, I could not cover everything but here is the presentation text which covers all the app functionalities and can be tested using this repo.

Demo Transcript:

Welcome to CS 291 Project 3 Demo video

This is my home page of the ruby on rails app called "Tweetbook". As you can see, it currently has no posts to display and we have links to some other endpoints.

Let's start the demo by navigating through supported endpoints as per the description on CS291 website.

"Navigating to the /users endpoint will list all users in your app". Let's test this.

As you can see, there are currently no users so the list is empty. Similar to this, I have created /comments endpoint which will list all comments in this app. We will come back to this later.

Let's create some users so we can test the rest of the basic requirements.
Let's create four users as follows:
1.ABC
2.PQR
3.IJK
4.XYZ
5.Test

As you saw during the creation, there is a validation error when you try to create or update user details when the required value is not provided.

Let's update the name of first user to abcd and change it's email.

Let's see if asking for user id 6 throws 404 error or not.

Let's delete the user "Test" successfully.

As you can see, after every action, "/users" gets updated accordingly. 

This completes the basic requirements mentioned on the website.

Let's create some posts
Title: First page on Tweetbook
Content: This is my first time here
User ID: 1

Title: Only page on Tweetbook
Content: This is my only time here
User ID: 2

Title: Second page on Tweetbook
Content: This is my second time here
User ID: 1

Title: Latest page on Tweetbook
Content: Hi I have just joined 
User ID: 3

Let's update the last Post with a smiley at the end.
Title: Latest page on Tweetbook
Content: Hi I have just joined :D
User ID: 3

Let's create some comments
Content: Hi everyone
User ID: 5
Post: 1

Content: Hi everyone
User ID: 5
Post: 2

Content: Welcome to Tweetbook
User ID: 1
Post: 2

Content: Hi everyone
User ID: 5
Post: 3

Content: Hi everyone
User ID: 5
Post: 4

Let's edit a comment to add !
Content: Welcome to Tweetbook!
User ID: 1
Post: 2

Let's see all the views now.
They all should be consistent.

Let's start deleting stuff.

Let's delete the user 4.

Let's delete the user 1.
As you can see. All it's posts and comments are gone.

Let me navigate through some part of the code.

Let's look at the models which are as per described in the specification.
One user will have many posts -> User ABC had 2 posts.
one post can have many comments -> Post "Only page on Tweetbook" had 2 comments which belonged to 2 different users.

Rest of the Code is available on github.

Thank you.
