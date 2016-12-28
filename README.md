# WE-MegaTest

## Problem Statement: Imagine you work for software offshore company, and your client ask you to create an application for advertisement posting.

You, as a developer, are required to implement the following.

1. User can post ads.
2. Each post can have the following attributes. (title, description, location, phone_number, user_id, category, status, posted_date, updated_date)
3. User Id of post should be automatically added based on session of currently logged in user.

4) Create an Admin panel where admin can edit/delete/approve user's ads.

## Flow of the Site.

When a visitor visits the site It will be redirected to front page which list top 10 most recent ads.

The main menu for anonymous users should be

Home | Login | Register 

And for Logged In user should be


Home | Logout | My Ads (My ads will show all ads created by logged in user. )

### Home page. 

It will be the same listing with one minor modification. It will show edit | delete with those ads which is created by the logged in user.

### My Ads

Add New Add [Should be linked to create ad form]
S.No. | Title | 	Action
 1	  iPhone	Edit|Delete. [Delete should delete ad using ajax]

### Logout: It will logout the user

### Register: Register will register user and insert into a database and assign  a 
role of poster | admin.

## Roles based Dashboard

There are two roles (Poster, Admin)

Poster will only add ads to the site and edit/delete his/her ads.
Admin will edit/delete/approve add.

Ads will only show on the site if it has been approved by admin.

## Database Model.

There should be at least three tables. Users, Ads, Categories.

Users and Ads tables should have status field to track active/approved status.
