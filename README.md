# SCA-Cloud-School
First assessment

Docker Hub repo: https://hub.docker.com/repository/docker/1407281106/sca-cloud-docker/general

## Deployment instructions

Creat a Git repository called SCA-Cloud_School.
Clone the repsitorty into your termial.

Setup a Nodejs Aplication.
Switch into a start branch - git checkout- b Stable
Create a folder called Docker.
Run npm init (App name: docker-sample, Entry point: app.js)
Run npm install express



Setup a Docker File


Build a docker image
Run docker build -t dockerdemo where dockerdemo is the name of your image.
Run docker run -p 4990:8080 -d dockerdemo
Go to your docker desktop to view and run the docker image .

```sh
docker build -t username/sca-cloud-docker
```


Push to Github
Run git add .
git commit -m "message" 
git push to push the docker folder to the SCA-GitHub repository created.



Push to Dockerhub
Create a repo in Docker Hub named sca-cloud-docker.
Run docker tag image-id yourhubusername/reponame:tag 
Run docker push yourhubusername/reponame:tag
```sh
docker push 1407281106/sca-cloud-docker
```


Feture branch
Check out to feature branch git checkout -b feature
Change the content of the index.html file to “Welcome to SCA Cloud School Application, this is my first assessment”
Build and run a docker image docker build -t docker-feature ,docker run -p 4990:8080 -d docker-feature n/b: we use a different port number
Run your generated image on the docker desktop, confirm on http://localhost:4990
Add, commit and push feature branch to GitHub.
Push to the same docker repository docker tag image-id:yourhubusername/reponame:tag , docker push yourhubusername/reponame:tag n/b: we use feature as a tag.
