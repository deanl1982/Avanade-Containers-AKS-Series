# Session 01
## Anatomy of a Container

**Use "docker build" to compile a new image from the dockerfile**

'docker build -t web-app-fe .'

**Create container from image**

'docker run -d -p 80:80 web-app-fe'