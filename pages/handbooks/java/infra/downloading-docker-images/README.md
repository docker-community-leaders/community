### Download Images

This tutorial uses a few Docker images and software.
Let's download them before we start the tutorial.

Download the file from [docker-compose-pull-images.yml](https://raw.githubusercontent.com/docker/labs/master/developer-tools/java/scripts/docker-compose-pull-images.yml) and use the following command to pull the required images:

```
curl -O https://raw.githubusercontent.com/docker/labs/master/developer-tools/java/scripts/docker-compose-pull-images.yml
docker-compose -f docker-compose-pull-images.yml pull --parallel
```

_NOTE_: For Linux, `docker-compose` and `docker` commands need `sudo` access.
So prefix all commands with `sudo`.

