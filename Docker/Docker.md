# Docker

## Building Images
--pull

1. Build from Dockerfile
```docker build -t image-name path```

- if Dockerfile isn't named `Dockerfile` use -f
```docker build -t image-name -f dockerfiletest .```

2. Difference between ENTRYPOINT and CMD
- `CMD` and `ENTRYPOINT` => directives to specify -> cmd run by default in built images
- If use `CMD` -> Docker will run command using the default `ENTRYPOINT` -> /bin/sh
like CMD is an arg for ENTRYPOINT
like `ENTRYPOINT` run `CMD` -> `/bin/sh /bin/date`
ex:
```
sudo docker build -t 02 .
sudo docker run 02
```

-  Override `CMD`
```
sudo docker run 02 /bin/hostname
95eb48c83dee
```

3. Exposing a Port in the Dockerfile
- in Dockerfile: EXPOSE 1234
- arg in docker run: -p 1234:1234












