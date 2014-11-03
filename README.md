Rails Workshop
==============

This project was created for conducting session in Rails Workshop covering following topics:
- Change the UI
- Change a route
- Database migration
- Add devise
- Add paperclip for uploads

Visit http://goravbhootra.github.io/rails_workshop for more details.


Gemfile:
gem install devise

$ rails generate devise:install

Generating user model:
$ rails generate devise user
$ rake db:migrate

http://localhost:3000/users/sign_up
http://localhost:3000/users/sign_in

You can add
<% if user_signed_in? %>
to the template. This will help to let us know whether devise is working or not. We can also add the link paths. This will allow us to get working links within our page.

new_user_session_path
will allow you to login and it will create a new session until you logout.

edit_user_registration_path
will allow us to change our password and delete our account.

destroy_user_session_path
will allow you to logout and it will destroy your current session.