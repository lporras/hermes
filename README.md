# Hermes Server

Hermes is a minimal path-finding developed in Ruby on Rails using as backend PostGIS.

Hermes is the great messenger of the gods in Greek mythology and additionally as a guide to the Underworld. An Olympian god, he is also the patron of boundaries and of the travelers who travel across them.

## Prerequisites

To run the project you will need PostgreSQL and PostGIS extension in your system, you can look in internet for guides like this for <a href="http://techblog.strange-quark.com/gis/postgis-installation">Ubuntu Linux</a>, or this for <a href="http://www.lincolnritter.com/blog/2007/12/04/installing-postgresql-postgis-and-more-on-os-x-leopard/">Mac OSX</a>

You will need postgresql library for Ruby:

   $ sudo gem install postgresql

## Initial Config

You can run the server locally:

    $ rake gems:install #=> Install required dependencies
    $ rake db:create #=> Create DB, edit config/database.yml for setup your DB configuration
    $ rake db:migrate #=> Create application database tables
    $ script/server #=> Start Rails App