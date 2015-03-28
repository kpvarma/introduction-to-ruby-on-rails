> [<< BACK: Create a rails Application and Configure it](step-2-configure-application.md)

> [>> NEXT: Setup Database and start the application](step-3-setup-database-and-start-application.md)


##### Create a rails application

Let us first create a rails application

`$ rails new books_store --skip-bundle`

*--skip-bundle* will tell rails not to fetch the ruby gems from internet and install them locally. I would like to configure more gems for our API before I fetch them.


##### Configure your first rails application

Now let us go ahead and configure our application so that we are ready to start our development. Let us learn new things as and when we see them.

As a first step, I would like to add rspec-rails gem to our application.

Add the following gems to Gemfile under the development and test group

```
group :development, :test do

  ...

  gem 'rspec-rails', '~> 3.0'
  gem "shoulda"
  gem "pry"

  ...
end
```

Your gemfile is a list of all gems that you want to include in the project. It is used with bundler (also a gem) to install, update, remove and otherwise manage your used gems.

rspec and shoulda will help us to do TDD and pry is a debugger

These gems are hosted in rubygems.org (primarily).
Now let us tell rails to fetch these gems from the server and install locally.

`$ bundle install`

Now let us install rspec helper files to our application.
We will use rspec generator to install the required files

`$ rails generate rspec:install`

Finally, let us remove the test folder. Instead We will use spec folder for writing test cases.

`$ rm -fr test/`

We are now ready with the testing framework
Let us run the tests

`$ rspec`

```
No examples found.

Finished in 0.00029 seconds (files took 0.18185 seconds to load)
0 examples, 0 failures
```

> [<< BACK: Create a rails Application and Configure it](step-2-configure-application.md)

> [>> NEXT: Setup Database and start the application](step-3-setup-database-and-start-application.md)


##### References

* http://stackoverflow.com/questions/14072880/whats-the-use-of-gemfile-in-rails
* http://bundler.io/
* http://rspec.info/
* https://github.com/rspec/rspec-rails




