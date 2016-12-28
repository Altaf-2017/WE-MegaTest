# WE-MegaTest. AdsPoster.com


## Problem Statement: 

Imagine you are working for software offshore company, and your client ask you to create an application for advertisement posting.

You, as a developer, are required to implement the following.

## Roles:

There should be two roles. Admin and Poster.

### Admin:

is responsible of managing users, ads, categories.
Also, admin can approve/disapprove ads. Activate user's status, block users.

### Poster:

is logged in users which can only post ads. On posting of ads the state of post shall be pending which can be approved by admin later on. Only then it will show on front page.

## Pages:

### Home page.

It will show latest 10 ads and a pagination to visit more.

### Admin Dashboard:

This page will be only accessible to site administrators and It will have the following sections.

User CRUD.
Ads: Edit/Delete and Approve only.
Categories CRUD.

### Poster Admin Area

Ability to add/edit/delete his/her ads.

## Some Considerations.

1. User can post ads.
2. Each post can have the following attributes. (title, description, location, phone_number, user_id, category, status, posted_date, updated_date)
3. User Id of post should be automatically added based on session of currently logged in user.

4. Create an Admin panel where admin can edit/delete/approve user's ads.

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

### Logout: 

It will logout the user

### Register: 

Register will register user and insert into a database and assign  a 
role of poster | admin.

## Roles based Dashboard

There are two roles (Poster, Admin)

Poster will only add ads to the site and edit/delete his/her ads.
Admin will edit/delete/approve add.

Ads will only show on the site if it has been approved by admin.

## Database Model.

There should be at least three tables. Users, Ads, Categories.

Users and Ads tables should have status field to track active/approved status.

## Constraints.

1. It is required to use object oriented PHP and PDOs to approach the solution.
2. You must use PSR-1 Coding guide and PSR-2 Coding style guide in your code.

## How to start.

Go ahead and fork the project. Once you forked the project clone it on your local machine.

Start working on the project. And push your modules gradually over the course of development.

At the end, once you are done with the project. Push all your code. And export your database and place it in Git repository and push it too.
