# go.afunderburg

## Local Setup

This guide assumes you have Docker installed and running. 
To develop locally within a Docker container:

Open a cmd window from the project root (go.afunderburg). Then, run a docker image with this directory mounted to the running container.

```
WINDOWS

docker run --rm -it --name go.afunderburg -p 8080:8080 -v %cd%:/go/src/go.afunderburg golang
```

```
LINUX

docker run --rm -it --name go.afunderburg -p 8080:8080 -v $PWD:/go/src/go.afunderburg golang
```

Within the container, you can run the example program (simple web server) using the following commands:

```
cd /go/src/go.afunderburg
go run example_server.go
```

Navigate to localhost:8080 to view the server in action!
