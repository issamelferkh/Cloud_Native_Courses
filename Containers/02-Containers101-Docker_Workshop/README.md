# Containers 101 - Docker

## Get Started
### Sample App
- Clone App srcs
- Create Dockerfile
- Build
```sudo docker build -t sample-app:1.0 .```
- Run
```sudo docker run -dp 3000:3000 sample-app:1.0```

### Update the App
- Update src/static.js.app.js
```
-                <p className="text-center">No items yet! Add one above!</p>
+                <p className="text-center">You have no todo items yet! Add one above!</p>
``` 

- Build
```sudo docker build -t sample-app:1.0 .```

- Run
```sudo docker run -dp 3000:3000 sample-app:1.0```

- Issue: `Bind for 0.0.0.0:3000 failed: port is already allocated.`

- Solution
  - Stop the container -> remove it -> run

### Push/Share the App
- Create repo -> Docker Hub
- Tag 
```sudo docker tag sample-app:1.0 issamelferkh/sample-app:1.0```
- Push
```sudo docker push issamelferkh/sample-app:1.0```


### Persist DB
- Keep todos data using Volumes (connect specific filesystem paths of the container to the host machine)
- Create volume
```sudo docker volume create todo-db```

- Stop, remove container and add volume
```sudo docker run -d -p 3000:3000 -v todo-db:/etc/todos issamelferkh/sample-app:1.0```

- Inspect Volume
```sudo docker volume inspect todo-db```


### 6: Use bind mounts
### 7: Multi-container apps
### 8: Use Docker Compose
### 9: Image-building best practices
### 10: What next?



## Help
- Resource: https://docs.docker.com/
- Delete all
sudo docker stop $(docker ps -qa); docker rm $(docker ps -qa); docker rmi -f $(docker images -qa); docker volume rm $(docker volume ls -q); docker network rm $(docker network ls -q) 2>/dev/null
