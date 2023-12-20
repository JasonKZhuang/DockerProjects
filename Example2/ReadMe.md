## open the termical run build command to build this new image with --tag or -t
```shell
  $ docker build -t docker-example:[version] .
```

## and run docker run command
```shell
  $ docker run --name container-docker-example --rm -d -p 3001:80 docker/example:v1.1
```

```shell
   $ docker login
   # re-tag or re-name the image 
   $ docker tag docker-example:v1.0 jasonzhuang5/docker-example:v1.0
   # push to docker hub
   $ docker push jasonzhuang5/docker-example:v1.0

```

