![Maxxidata](https://camo.githubusercontent.com/5e9ffa46a7213e9e65e733ed2f7b1bb4554490c486846386515c885ae949fefd/68747470733a2f2f692e706f7374696d672e63632f715258545a5a307a2f6c6f676f2d332e706e67)

# JavaScript Engineer Challenge
**Welcome to our JavaScript Engineer Challenge**

This Challenge consists of a series of tasks which
may take between 4–6 hours to complete, depending
on your experience level. The primary purpose of
this test is to infer your “logical thinking”
and “problem-solving” skills.

## Summary
- [Scenario](#scenario)
- [Getting Started](#getting-started)
- [Backend](#backend)
- [Frontend](#frontend)
- [Extras](#extras)
- [Tips](#tips)
- [Deadline](#deadline)
- [Submissions](#submissions)

## Scenario
We want you to create an application for managing
users. The application must meet the following
requirements:

1. Create new users;
1. List users;
1. Edit users;
1. Delete users;


## Getting Started
Fork this repository (to jump-start your test) and
run `npm install` on both the `/api` and `/front`
directories, then follow the requirements for the
[Backend](#backend) and [Frontend](#frontend) when
developing your application.

Feel free to use any library you are used to or
to create things your way. Just keep in mind
the required frameworks for the frontend and
backend, confirm if the library you will use
don't have any problems with it.

## Backend
To create the backend of this application we
want you to use [Nest.js](https://nestjs.com/)
as the framework. It's ok not knowing all the
perks of the framework, but we want to see how
you manage to work with it.

Your backend must meet the following requirements:

1. It has to use a relational database
   (PostgreSQL, MySQL, MariaDB, etc...);
1. The user needs to have one relation, being the
   "user_type";
1. It needs to have unit tests;
1. Your API needs to have a CRUD for the users;
1. Your API needs to have validations for the fields:
   1. Only boolean for `active` fields;
   1. Only valid e-mails for `email` fields;
   1. Max size of 255 for `string` fields;
   1. Only `UUID` for `id` fields;
1. Your API needs to follow the patterns of a
   REST implementation;

### Data models
`user_type`

```json
{
  "id": "a8d7f-1j4...",   // required
  "description": "test",  // required
  "active": true,         // required
  "updatedAt": "",        // required
  "createdAt": ""         // required
}
```

`user`

```json
{
  "id": "a8d7f-1j4...",       // required
  "nickname": "test",         // required
  "name": "test",             // required
  "phone": "99999999999",
  "email": "email@test.com",  // required
  "user_type": 999,           // required (relation)
  "active": true,             // required
  "updatedAt": "",            // required
  "createdAt": ""             // required
}
```


## Frontend
To create the frontend of this application we
want you to use [Angular](https://angular.io/)
with [Angular Material](https://material.angular.io/)
as the framework. It's ok not knowing all the
perks of the framework, but we want to see how
you manage to work with it.

Your frontend must meet the following requirements:

1. It has to communicate with your backend;
1. It has to have a home page with a side menu and
   a list of users;
1. It has to have a route to create/edit a user;
   1. When creating/editing the `submit` button
    needs to be disable until all required fields
    are validated;
1. It has to have a route to detail the user;
1. It has to have a route to delete the user;
    1. When deleting a user, it should ask
    for confirmation. The button to confirm
    needs to be `disabled` until the nickname
    of the user being deleted is informed
    and validated (like the deletion of
    repositories in Github).

It's up to you how you will define the frontend
layout, if you will use new pages of modals for
each interaction.

## Extras
There are some extras we would like to see in
your repository. These aren't required, feel 
free to include them or not.

- Use an authentication method (like `OAuth`);
- Use something to register logs from your
  application (like `Winston` with `Redis`);
- Generate a `Docker` image with `Docker Compose`
  and the required `migrations` and `seeders`
  (if you don't use `Docker` in your application,
  please make sure to include on the repository an
  `database dump`).

## Tips
- Keep it simple
- Please ensure your readme file contains valid and simple instructions
- Please use placeholder data only (i.e. do not use real or identifiable information)
- Feel free to validate fields according to your own validation logic
- Verify the full functionality of your application prior to submission
  

## Deadline
Please submit your test as a Github repository
URL, along with a readme file containing
instructions on how to set up and run your
application. If you'd like to submit a
_private repository_, please add
[Raphael](https://github.com/raphaeljp)
with view access to the private repository.

The deadline for submission is
**7 days after you receive this challenge**.

_Submissions will not be accepted after this date._


## Submissions
Submit the repository URL to the person who asked you to take this challenge.

If you have any doubts, please submit them to [rh@maxxidata.com](rh@maxxidata.com).


[Back to the top](#javaScript-engineer-challenge)
