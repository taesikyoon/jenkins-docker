[jenkins docs](https://www.jenkins.io/doc/book/installing/docker/)
[jenkins image hub](https://hub.docker.com/_/jenkins/tags)
[jenkins docker git](https://github.com/jenkinsci/docker)
[jenkins master/slave](https://medium.com/@yassine.essadraoui_78000/jenkins-docker-in-docker-b7630c7b9364)

### Jenkins docker start

```
docker build -f Dockerfile-master -t jenkins .
docker run -dit --restart=always -p 8080:8080 -p 50000:50000 -v jenkins_home:/var/jenkins_home -v /var/run/docker.sock:/var/run/docker.sock jenkins

```
