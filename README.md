Introduction
------------

This is a fully-featured image for Stockfish testing framework client.


Quick start
-----------

Create an empty directory and extract management scripts:

```
mkdir fishtest-client
cd fishtest-client
docker run -it --rm --name fishtest-client skiminki/fishtest-client scripts | bash
```

Rename config.sh.template to config.sh and fill in your USERNAME and
PASSWORD for Stockfish testing framework:

```
mv -iv config.sh.template config.sh
vim config.sh
```

Start the container:

```
./start-fishtest-worker.sh
```

To stop after the current testing batch has completed: (may take a while)

```
./stop-fishtest-worker.sh --wait
```


Built-in help:
--------------

Use the following command for built-in help:
```
docker run -it --rm skiminki/fishtest-client help
```


Links:
------

- Stockfish testing framework: https://tests.stockfishchess.org/
- Docker hub repository: https://hub.docker.com/repository/docker/skiminki/fishtest-client
- GitHub repository for building the Docker image: https://github.com/skiminki/fishtest-client-docker
