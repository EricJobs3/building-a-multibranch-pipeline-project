

## Run Jenkins/BlueOcean locally
```
docker run \                                                           
  --rm \
  -u root \
  -p 8080:8080 \
  -v jenkins-data:/var/jenkins_home \
  -v /var/run/docker.sock:/var/run/docker.sock \
  -v "$HOME":/home \
  jenkinsci/blueocean
  ```

## Jenkinsfile-dockerfile build image on the fly
`Jenkinsfile-dockerfile` add customerized env files in dockerfile
