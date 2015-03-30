> [<< 2. Create a rails Application and Configure it](step-2-configure-application.md)

> [>> 4. Write the User Story](step-4-write-user-story.md)


### Setup Database and Start Application

We now have a bare minimum skeleton rails application which is working. Let us setup the database

```
|-> demo-application
..
..
|-> db
  |-> migrate
    |-> 20150322110343_create_books.rb
  |-> schema.rb
  |-> seed.rb
..
..

```

Let us create the database file (in our case it is [SQLite3][sqlite3]) and run the migrations

`$ rake db:create db:migrate`

Now, start the application

`$ rails s`

This will now invoke bin/rails script which is responsible for spawning a webrick which is a web server.
Webrick will by default listen to localhost:3000

> you can change the port by passing -p 3001.

Let us see what our application look like.

Open up a browser and type localhost:3000 and hit enter
you will see a getting started page.

Yay. we are done with Step 3 - few more to go.

> [<< 2. Create a rails Application and Configure it](step-2-configure-application.md)

> [>> 4. Write the User Story](step-4-write-user-story.md)


##### References

* http://www.tutorialspoint.com/ruby-on-rails/rails-directory-structure.htm
* http://stackoverflow.com/questions/9884429/rails-what-does-schema-rb-do
* http://guides.rubyonrails.org/active_record_migrations.html

[sqlite]: https://www.sqlite.org/





