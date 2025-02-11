RACHEL GRIFFITHS
=================

## CHALLENGE: INSTAGRAM
------------
* Build Instagram!

##### BUSINESS LOGIC
------------
* USERS can post PICTURES
* USERS can write COMMENTS on pictures
* USERS can LIKE pictures
* USERS can filter pictures

##### WEB INTERFACE
* Style it like Instagram's website (or more awesome!)
* [Instagram Official](https://www.instagram.com)

### TECHNOLOGIES
------------

##### BACKEND
* Ruby On Rails - Web Application Framework
* Devise - Gem that builds user authentication functionality, creating sign up, sign in and sigh out features for Users
* Database: Postgres

##### FRONTEND
* HTML
* CSS
* Bootstrap

### GETTING STARTED
------------
* Clone the following repo: git@github.com:rachjgriff/instagram-challenge.git
* Run the following in your command line:

```bash
> bundle install
> bin/rails db:create
> bin/rails db:migrate

> bundle exec rspec # Run the tests to ensure it works
> bin/rails server # Start the server at localhost:3000
```

### TESTING
------------
* RSpec - Testing Framework
* Rubocop - Linter
* SimpleCov - Test Coverage
* Travis - CI

### WEB REQUIREMENTS
------------
##### USERS
- [ ] User can sign up with username, email address and password
- [ ] User can sign in
- [ ] User can sign out
- [ ] User details are stored in a database
- [ ] User is redirected to sign up/sign in page if not logged in
- [ ] User can edit their profile
- [ ] User can add a photo to their profile

  ###### CONFIRMATION SIGN UP / SIGN IN FEEDBACK
  - [ ] User receives confirmation via webpage if successfully signed up
  - [ ] User receives confirmation via webpage if successfully signed in

  ###### INCORRECT SIGN UP FEEDBACK
  - [ ] User receives feedback via webpage if sign up is unsuccessful due to invalid email
  - [ ] User receives feedback via webpage if sign up is unsuccessful due to email already being taken
  - [ ] User receives feedback via webpage if sign up is unsuccessful due to password criteria not met
  - [ ] User receives feedback via webpage if sign up is unsuccessful due to password not matching password confirmation

  ###### INCORRECT SIGN IN FEEDBACK
  - [ ] User receives feedback via webpage if sign in is unsuccessful due to invalid email
  - [ ] User receives feedback via webpage if sign in is unsuccessful due to email not being recognised
  - [ ] User receives feedback via webpage if sign up is unsuccessful due to email and password combination is incorrect

##### PICTURES
- [ ] User can upload picture
- [ ] User can delete picture
- [ ] Pictures are stored in a database against the user id (one-to-many relationship)
- [ ] Pictures are displayed on a web page with the user's username against it

##### COMMENTS
- [ ] User can leave a comment against a picture
- [ ] User can delete a comment
- [ ] Pictures can have multiple comments against them from different users or the same user
- [ ] Comments are stored in a database (one-to-many relationship)

##### LIKES
- [ ] User can 'like' a picture
- [ ] User can 'unlike' a picture
- [ ] Pictures can have multiple 'likes' against them from different users
- [ ] Likes are stored in a database (one-to-many relationship)

### APPROACH
------------
1. Setup project file with required frameworks  

2. Breakdown business logic provided into web requirements

3. Diagram instagram database:

![Database](images/instagram_database_diagram.jpg)

4. Follow the following article as a guide:[Build Instagram by Ruby On Rails Part 1](https://medium.com/luanotes/build-instagram-by-ruby-on-rails-part-1-fef7837ee399)

  STEPS TAKEN SO FAR:
  1. Install Rails
  2. Create a new rails project
  3. Bundle install
  4. Create a homepage and set it to your index route
  5. Configure database
  6. Create database
  7. Install bootstrap and set up styling sheets
  8. Implement layout: Navigation bar, main content, footer
  9. Install devise (setup user authentication)
  10. Setup devise
  11. Create User model

### FOLLOW UP

* Continue to work through the article to understand how Rails works

------------
Instagram Challenge
===================

## Instructions

* Challenge time: one weekend
* Feel free to use Google, your notes, books, etc., but work on your own
* If you refer to the solution of another coach or student, please put a link to that in your README
* If you have a partial solution, **still check in a partial solution**
* You must submit a pull request to this repo with your code by 9am Monday morning

## Task

Build Instagram: Simple huh!

Your challenge is to build Instagram using Rails. You'll need **users** who can post **pictures**, write **comments** on pictures and **like** a picture. Style it like Instagram's website (or more awesome).

Bonus if you can add filters!

## How to start

1. Produce some stories, break them down into tasks, and estimate
2. Fork this repo, clone, etc
3. Initialize a new rails project

Remember to proceed in small steps! Getting confused? Make the steps even smaller.

## Code Quality

For linting, you can use the `.rubocop.yml` in this repository (or your own!).
You'll need these gems:

```ruby
gem "rubocop", "0.48.1"
gem "rubocop-rails"
```

You can also lint Javascript, CSS, and ERB — feel free to research this. These
will help you to train yourself to produce cleaner code — and will often alert
you to mistakes or mishaps!
