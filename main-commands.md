# Main Commands

## Show Images

```
$ docker images		# Intermediate Images will `NOT` be visible
$ docker images -a
$ docker images --format '{"ID":"{{ .ID }}", "Image": "{{ .Image }}", "Names":"{{ .Names }}"}' # shows images output as JSON
```

## Delete an Image

With `docker rmi`:
```
$ docker rmi IMAGE_ID [IMAGE_ID...]
```

With `docker image rm`:

```
$ docker image rm IMAGE_ID [IMAGE_ID...]
```

## Show Containers

```
$ docker ps				# will only show the running containers.
$ docker container ls	# will only show the running containers.

$ docker ps -a 			# Will show all containers
$ docker container ls -a 			# Will show all containers
```

## Remove Containers



## Pull Image and then Run

```
$ docker pull postgres:9.6
$ docker run -d postgres:9.6
```

### Specifying Ports

```
$ docker run -d -p 5432:5432 postgres:9.6
```

> If you want only accessible from localhost:

```
$ docker run -d -p 127.0.0.1:5432:5432 postgres:9.6
```

## Automatically Remove the Container when It Exits

### Pull Curl

```
$ docker pull curlimages/curl:7.79.1
```

### Checking Curl Version

```
$ docker run --rm curlimages/curl:7.79.1 --version
```

### Follow Location(-L) and Verbose(-v) with Curl

```
$ docker run --rm curlimages/curl:7.79.1 -L -v http://www.google.com
```

## 