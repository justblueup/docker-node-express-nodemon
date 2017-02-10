# docker-node-express-nodemon
I created this app to test editing a running docker image from the local host on a mac.  The docker image will mount the local app directory into the image so that you can edit from the local machine.  Nodemon will detect the changes and restart the node server in the docker image.  The app is run using docker compose.

### Install
You must have docker installed on your local machine.  Docker for mac can be downloaded here:  [Get Docker](https://www.docker.com/products/overview) Then just clone repo and cd into directory

### To run app use docker-compose
`docker-compose up`

While the app is running the image will bind to the host port 3000 on the local machine.  To view hello world go to

`http://localhost:3000`

You may then edit app.js on the local host.  Nodemon will detect changes and restart the node server in the image.

###To stop the node server

`control-c` 

###To quit the app

`docker-compose down`

This will remove the container.
