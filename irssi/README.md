# Irssi

Getting started:

```
docker build --tag irssi .
```

And binary to run the container from CLI:

```
#!/bin/sh

docker run -it --rm --name jirssi -e TERM -u $(id -u):$(id -g) \
    --log-driver=none \
    -v $HOME/.irssi:/home/user/.irssi:rw \
    irssi
```
