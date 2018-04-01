ICF Literature
================

This is a sample Ruby on Rails application generated for the Docker class at Frisco Masjid.

Local Setup (without docker)
---------------------------

* First install the latest version of ruby > 2.4

* Install a javascript runtime (nodejs, for example): `apt-get install nodejs`

* Install the rails gem `gem install rails`

* Install the mysql database. See [mysql](https://dev.mysql.com/doc/refman/5.7/en/installing.html)

* Set up your mysql username and password in `config/database.yml`

* Clone this repository `git clone https://github.com/faraazkhan/icf-literature.git`

* Install all gems `cd icf-literature; bundle install`

* Create the database: `bundle exec rake db:create`

* Run all rails migrations: `bundle exec rake db:migrate`

* Start the server: `bundle exec rails s`

Goals
-----

Your goal is to dockerize this application and run it as a three tier application one image each for:

* nginx
* rails
* mysql
