# Docker NGINX Angular Example
Example passing env variables from docker to Angular appication and deploy to NGINX container.

# Install
1) Install dependecies

    `cd src/a/`

    `npm install`
2) to genereate `dist/` folder

    `ng build`

3) go back to Dockerfile directory

    `cd ../..`


4) the root folder contains a Dockerfile, to build the Image:

    `docker build -t server .`

5) to run the image use the parameters below:

    `docker run -p 80:80 -d --name server -e title='Tittle Variable from Docker' server`
    
6) Check in some browser: `http:\\localhost`
