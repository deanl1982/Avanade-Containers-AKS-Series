## Common Docker Commands

1. **docker run**:
   - *Explanation*: Runs a command in a new container.
   - *Common Switches*:
     - `-d`: Detached mode (run container in the background).
     - `-it`: Interactive mode (attach STDIN, STDOUT, STDERR).
     - `--name`: Assign a name to the container.
     - `-p`: Publish container's ports to the host.
     - `-v`: Bind mount a volume.

2. **docker ps**:
   - *Explanation*: Lists running containers.
   - *Common Switches*:
     - `-a`: Show all containers (including stopped ones).
     - `-q`: Only display container IDs.

3. **docker images**:
   - *Explanation*: Lists available images.
   - *Common Switches*:
     - `-a`: Show all images (including intermediate images).
     - `--filter`: Filter output based on conditions.

4. **docker build**:
   - *Explanation*: Builds an image from a Dockerfile.
   - *Common Switches*:
     - `-t`: Name and optionally a tag in the 'name:tag' format.
     - `--build-arg`: Set build-time variables.

5. **docker pull**:
   - *Explanation*: Pulls an image from a registry.
   - *Common Switches*:
     - None

6. **docker push**:
   - *Explanation*: Pushes an image to a registry.
   - *Common Switches*:
     - None

7. **docker stop**:
   - *Explanation*: Stops a running container.
   - *Common Switches*:
     - None

8. **docker rm**:
   - *Explanation*: Removes one or more containers.
   - *Common Switches*:
     - `-f`: Force removal of a running container.

9. **docker rmi**:
   - *Explanation*: Removes one or more images.
   - *Common Switches*:
     - `-f`: Force removal of the image.

10. **docker exec**:
    - *Explanation*: Run a command in a running container.
    - *Common Switches*:
      - `-it`: Interactive mode.
      - `-u`: Specify the username or UID.

## Docker Compose Commands

1. **docker-compose up**:
   - *Explanation*: Builds, (re)creates, starts, and attaches to containers for a service.
   - *Common Switches*:
     - `-d`: Detached mode.
     - `--build`: Build images before starting containers.
     - `--force-recreate`: Recreate containers even if their configuration and image haven't changed.

2. **docker-compose down**:
   - *Explanation*: Stops and removes containers, networks, volumes, and images created by `docker-compose up`.
   - *Common Switches*:
     - `-v`: Remove volumes.
     - `--rmi`: Remove images. Allowed values: 'all', 'local', 'none'.

3. **docker-compose build**:
   - *Explanation*: Builds or rebuilds services.
   - *Common Switches*:
     - None

4. **docker-compose pull**:
   - *Explanation*: Pulls images for services defined in a docker-compose.yml file.
   - *Common Switches*:
     - None

5. **docker-compose exec**:
   - *Explanation*: Run a command in a running container.
   - *Common Switches*:
     - None