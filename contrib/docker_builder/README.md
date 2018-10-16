# Dockerfile for building goldpressedlatinum binaries.

Now, you can build your own goldpressedlatinum files on all systems with docker and do it easy without installing depends on your system.

## How:

### Build docker image

```
sudo docker build .
```

### Run docker container

Builder will return HASH of image
Example:
Successfully built 9bbff825d50f

```
sudo docker run -it -v ~/path/to/goldpressedlatinum/folder:/goldpressedlatinum 9bbff825d50a
```

If your system uses SELINUX you may use --privileged=true key

```
sudo docker run --privileged=true -it -v ~/development/goldpressedlatinum:/goldpressedlatinum 9bbff825d50a
```

See goldpressedlatinum-qt file in used goldpressedlatinum folder and goldpressedlatinumd file in src subfolder.