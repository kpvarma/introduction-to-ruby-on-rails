# Configure your first rails application

Now let us go ahead and configure our application so that we are ready to start our development. I will be explaining about some parts of the project code rails has created us, as and when we cover them.

As a first step, I would like to add rspec-rails gem to our application.

Add the following gems to Gemfile under the development and test group

group :development, :test do

  ...

  gem 'rspec-rails', '~> 3.0'
  gem "shoulda"
  gem "pry"

  ...
end

# EXPLAIN about Gemfile
# Add link to migrations page of railsguides

rspec and shoulda will help us to do TDD and pry is a debugger

These gems are hosted in rubygems.org (primarily).
Now tell, rails to fetch these gems from the server and install locally.

$ bundle install

Now let us install rspec helper files to our application.
We will use rspec generator to install the required files

$ rails generate rspec:install

Finally, let us remove the test folder. Instead We will use spec folder for writing test cases.

$ rm -fr test/

We are now ready with the testing framework
Let us run the tests

$ rspec

No examples found.

Finished in 0.00029 seconds (files took 0.18185 seconds to load)
0 examples, 0 failures




