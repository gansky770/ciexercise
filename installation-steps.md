# Installing Jenkis docker style
```
$ docker run -tid -p 8080:8080 -p 5000:5000 --volume jenkins_home:/var/jenkins_home --volume /var/run/docker.sock:/var/run/docker.sock --name jenkins  jenkins/jenkins:lts-jdk11
```



