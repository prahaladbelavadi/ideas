# Using github as a CMS

## Abstract

Most static site generators generate the html to be rendered before pushing to github remotes.
Github repository remotes can be configured to be hosted as sites via github pages.

For applications that require external apis, they can be called when the pages are rendered or when they are compiled.

In order to host a backend cms, you'll need an ec2 instance to host the server that sends api data. 
That can be replaced with github.
Github itself can serve files as json. [ref](https://victorscholz.medium.com/hosting-a-json-api-on-github-pages-47b402f72603)

Applications like ghost can be served via github pages. For public repositories, the login checks such as username and password can be hashed when stored.
This implies that the hash of the password is in the public domain and can be subject to dictionary attacks or compared against a list of exposed, precompiled password.

But you can effectively create an entire system, frontend, backend and the interworkings over github.
There is also a possibility where the backend could be served from a json file hosted on github pages. Changes to the contents of the json files would result in the response changing.
There can be an open api specification that also compiles into a github api application.
