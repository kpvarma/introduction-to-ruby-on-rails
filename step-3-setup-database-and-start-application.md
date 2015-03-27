# We now have a bare minimum skeleton rails application which is working.
# Let us setup the database

# EXPLAIN db folder, migration (version, up and down)
# Add link to migrations page of railsguides

$ rake db:create db:migrate

Let us start the application

# EXPLAIN about schema.rb

$ rails s

This will now invoke bin/rails script which is responsible for spawning a webrick which is a web server.
Webrick will by default listen to localhost:3000

# you can change the port by passing -p 3001.

Let us see what our application look like.

Open up a browser and type localhost:3000 and hit enter
you will see a getting started page.

Yay. we are done with Step 3 - few more to go.







