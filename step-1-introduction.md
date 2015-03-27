# Pre-requisite

I am not covering installation steps during this session.
I have added a commeent in the meetup.com page which has links to installation guides. (Both Ruby and Rails)
I can also share the links again with you all via email.

In this session I will be covering about

1) Creating a rails application from scratch and configuring required gems for test driven development

2) Showing how to create a simple book store API which will accept a GET request to URL /api/v1/books.json and returns a the json containing the list of books

3) While developing the application, I will be following Test Driven Development (TDD). i.e, I will write a test case for a feature and then develop the application.

# Check if you have installed ruby and rails properly

$ ruby -v (in linux, mac)
ruby 2.1.2p95 (2014-05-08 revision 45877) [x86_64-darwin13.0]

$ rails -v (in linux, mac)


# Create rails application

Let us first create a rails application

$ rails new books_store --skip-bundle

--skip-bundle will tell rails not to fetch the ruby gems from internet and install them locally. I would like to configure more gems for our API before I fetch them.


