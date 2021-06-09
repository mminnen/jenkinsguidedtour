## Jenkins Guided Tour
https://www.jenkins.io/doc/pipeline/tour/getting-started/

## use a Jenkins container for testing
Install Jenkins on Windows:
https://www.jenkins.io/download/thank-you-downloading-windows-installer-stable/

## use a Jenkins container for testing
https://github.com/jenkinsci/docker/blob/master/README.md

```bash
docker pull jenkins/jenkins:lts
docker run -p 8080:8080 -p 50000:50000 -v jenkins_home:/var/jenkins_home jenkins/jenkins:lts
```

This will automatically create a 'jenkins_home' docker volume on the host machine. Docker volumes retain their content even when the container is stopped, started, or deleted.

Access Jenkins Container at: http://127.0.0.1:8080/

