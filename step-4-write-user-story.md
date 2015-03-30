> [<< 3. Setup Database and start the application](step-3-setup-database-and-start-application.md)

> [>> 5. Write the first Request Spec](step-5-write-the-first-request-spec.md)


### Write User Story

It is time to do some real action.
Let us set some expectations

##### What is a User Story

A [user story][user-story] is a tool used in Agile software development to capture a description of a software feature from an end-user perspective. The user story describes the type of user, what they want and why. A user story helps to create a simplified description of a requirement.

> As an API user, when I send a request to /api/v1/books.json, I should be able to get a books json data

I have the json format defined here already which is like:

[Click here to download books.json](json/books.json)
```
{
  "books": [
    {
      "id": 1,
      "name": "The Merchant of venice",
      "author": "William shakespeare",
      "isbn": "9781467758567",
      "description": "The Merchant of Venice is a play by William Shakespeare in which a merchant in 16th century Venice must default on a large loan provided by an abused Jewish moneylender. It is believed to have been written between 1596 and 1598."
    },
    {
      "id": 2,
      "name": "My experiments with Truth",
      "author": "Mahatma Gandhi",
      "isbn": "9781607960201",
      "description": "The Story of My Experiments with Truth is the autobiography of Mohandas K. Gandhi, covering his life from early childhood through to 1921. It was written in weekly instalments and published in his journal Navjivan from 1925 to 1929."
    },
    {
      "id": 3,
      "name": "The Cairo Trilogy",
      "author": "Naguib Mahfouz",
      "isbn": "9780375413315",
      "description": "Naguib Mahfouz's magnificent epic trilogy of colonial Egypt appears here in one volume for the first time. The Nobel Prize--winning writer's masterwork is the engrossing story of a Muslim family in Cairo during Britain's occupation of Egypt in the early decades of the twentieth century."
    }
  ]
}
```


Now we have expectation set. Let us start developing the applicaiton.

> [<< 3. Setup Database and start the application](step-3-setup-database-and-start-application.md)

> [>> 5. Write the first Request Spec](step-5-write-the-first-request-spec.md)

##### References

* http://en.wikipedia.org/wiki/User_story
* https://help.rallydev.com/writing-great-user-story
* https://www.scrumalliance.org/community/articles/2010/april/new-to-user-stories

[user-story]: http://en.wikipedia.org/wiki/User_story
