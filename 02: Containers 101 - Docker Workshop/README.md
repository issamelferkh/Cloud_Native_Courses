# Containers 101 - Docker

- Ressoucre: https://docs.docker.com/get-started/
## Sample application
Deploy sample node app using our 1st Dockerfile
1. Create Dockerfile
2. Build
``` docker build -t sample-app. ```
3. Run
``` docker run -dp 3000:3000 sample-app ```

## Update App
1. Update srcs
2. Stop and Remove Container
3. Build
4. Run

## Push/Share App
1. Create repo in Docker Hub
2. Tag image
to give `sample-app` image new name
3. Push

## Persist Data
1. Create Volume
```docker volume create todo-db```
2. Run the container adding volume
```docker run -dp 3000:3000 -v data-db:/etc/todos sample-app```
3. Inspect Volume
```docker volume inspect todo-db```