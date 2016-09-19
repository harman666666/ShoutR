# ShoutR
The backend NodeJS Web API for the StreetRep Messaging Application.

The web API stores messages and other user information in Firebase. 
The API was deployed on Heroku at this link:
https://shout-r.herokuapp.com/

For more information on the application go here:
https://github.com/harman666666/StreetRep


The endpoints for the API are:

GET: https://shout-r.herokuapp.com/posts
Gets all the posts

GET: https://shout-r.herokuapp.com/posts/{post-id}
Gets the post with that post-id

GET: https://shout-r.herokuapp.com/users/{username}/posts
Gets all the posts made by the user with the specified username

POST: https://shout-r.herokuapp.com/posts/message
Creates a new message taking this type of JSON:

{
"username": "harman",
"message": "hello world",
"latitude": "500",
"longitude": "60"
}

POST: https://shout-r.herokuapp.com/users/create
Creates a new users taking this type of JSON:

{
"username": "harman",
"firstName": "hello world",
"lastName": "500",
}

POST: https://shout-r.herokuapp.com/posts/rankup/{post-id}
Increases the rating of the post with specified post-id by 1

POST: https://shout-r.herokuapp.com/posts/rankdown/{post-id}
Decreases the rating of post with specified post-id by 1











