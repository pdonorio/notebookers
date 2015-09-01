
### Containers to run your IPython py3k Notebooks with Docker

#### Pre-requisites

Install [docker](https://www.docker.com/whatisdocker) and [docker compose](https://docs.docker.com/compose/) tool.

Those tools come bundle for mac/windows in the new [docker toolbox](https://www.docker.com/toolbox).

#### Running

From a terminal shell

```
$ git clone https://github.com/pdonorio/notebookers.git

$ cd notebookers/containers

$ docker-compose -f containers/bootstrap.yml up
```

The first bootstrap (only) will take longer as the image will build.

The notebook service will start on `port 80`.

Then you may visit your [localhost](http://localhost) web page.
In case of docker based on virtualbox (or other VM) you should use
your VM IP instead of localhost.

### TO DO

Publish the image as automatic build with the new docker hub.

The reason why i waited is that to point to a Dockerfile,
you cannot use a personal name. ***Meh***