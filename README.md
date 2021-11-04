# Antlr4 Docker container

![Build](https://github.com/Any0ne22/antlr4-docker/actions/workflows/docker-image.yml/badge.svg)
![LatestVersion](https://img.shields.io/github/v/tag/Any0ne22/antlr4-docker?label=Latest%20version)
![DockerVersion](https://img.shields.io/docker/v/any0ne22/antlr4?label=docker%20version)

This repository is used to build automatically new releases of [Antlr4](https://github.com/antlr/antlr4/) and publish them to the Docker hub (at [any0ne22/antlr4](https://hub.docker.com/repository/docker/any0ne22/antlr4)).

## Usage

```bash
docker run --rm -u $(id -u ${USER}):$(id -g ${USER}) -v `pwd`:/work any0ne/antlr4:latest java -Xmx500M -cp /usr/local/lib/antlr4-tool.jar org.antlr.v4.Tool -o src/ -Dlanguage=Java grammar.g4
```

