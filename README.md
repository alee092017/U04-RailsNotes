# U04-RailsNotes for WDI

1.  rails new "AppName" -G --database=postgresql
  - **"-G" if your directory is already a git repo**
  - "--database" specifies which db prgrm to use. 
  
2.  cd into App
3.  Bundle Install
4.  rails db:create
5.  *Add & Commit everything*
6.  rails g model "Modelname"-should be *capitalized & singluar*
     - db/migrate--->open the migration
     - define columns in table using:
          t.datatype :columname
5.  add & commit the migration 
5.  rails db:migrate
      - see db/schema.rb
5.  For the balance of db tables, repeat previous two steps
      - add & commit db/schema.rb
6.  rails db:seed

Refer to:
  How to determine the sequence to run your migratations--is it left to right?  what if 

  [Active Record Basics from the Ruby on Rails Docs](http://guides.rubyonrails.org/active_record_basics.html)
  
  [on Nokogiri](https://codedump.io/share/tpZIx2NrDD6v/1)
