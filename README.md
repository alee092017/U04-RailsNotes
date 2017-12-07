# U04-RailsNotes for WDI

## setup:
1.  rails new "AppName" -G --database=postgresql
  - **"-G" if your directory is already a git repo**
  - "--database" specifies which db prgrm to use.  
2.  cd into App
3.  Bundle Install

[plurals/caps](https://git.generalassemb.ly/wdi-nyc-thundercats/LECTURE_U04_D05_Active-Record#pluralization)

## migrations:
### root/db
4.  rails db:create
5.  *Add & Commit everything*
6.  rails g model "Modelname"-should be *capitalized & singluar*
     - db/migrate--->open the migration
     - define columns in table using:
          t.datatype :columname
7.  *add & commit the migration*
8.  rails db:migrate
      - see db/schema.rb
9.  For the balance of db tables, repeat previous two steps
      - *add & commit db/schema.rb*
10.  rails db:seed
11.  more mistakes and typoes
12.  repeat all above

## relationships:
## app/models

[Active Record Associations](http://guides.rubyonrails.org/association_basics.html#choosing-between-has_many-through-and-has_and_belongs_to_many)

[from wdi lecture](https://git.generalassemb.ly/wdi-nyc-thundercats/LECTURE_U04_D05_Active-Record#relations-and-models)

13.  model.rb
     - relationship :table or :row (?) am i understanding that correctly?
     - *add & commit*
14.  indexing--


## seeds/seeding:
## root/db
14.  create seed file...
[ruby docs](http://edgeguides.rubyonrails.org/active_record_migrations.html#migrations-and-seed-data)
[seeding from csv...](https://gist.github.com/arjunvenkat/1115bc41bf395a162084)


# Random references/reminders:
  - Work in branches otherwise you'll have to start over for the 35th fucking time.
  
  - reminder git push origin branchname
  - replace a migration with an effing typo in it rails g model Thing --force
      - adverse effects?  is it really ok to do this?
  
  - How to determine the sequence to run your migratations--is it left to right?  what if 

  - [Active Record Basics from the Ruby on Rails Docs](http://guides.rubyonrails.org/active_record_basics.html)
  - [commands from lecture](https://git.generalassemb.ly/wdi-nyc-thundercats/LECTURE_U04_D05_Active-Record#commands-to-know)
  - [db commands](https://jacopretorius.net/2014/02/all-rails-db-rake-tasks-and-what-they-do.html)
  - [on Nokogiri](https://codedump.io/share/tpZIx2NrDD6v/1)
