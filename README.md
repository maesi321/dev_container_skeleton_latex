# Dev container skeleton with LaTeX
A skeleton project for creating LaTeX documents with VS Code dev container. 

## Motivation
The motivation for this project was to learn about VS Code Dev Container and Docker. Maybe it will help someone as a stepping stone for their own project.

This project is far from being production ready. There is also a lot of room for improvement in terms of performance.

## Resources
- [Dockerfile reference](https://docs.docker.com/reference/dockerfile/)
- [Docker-compose reference](https://docs.docker.com/reference/compose-file/)
- [VS Code dev container reference](https://code.visualstudio.com/docs/devcontainers/containers)
- [LaTeX quick start](https://latex-tutorial.com/quick-start/)


## Other skeletons
- [React and FastAPI](https://github.com/maesi321/dev_container_skeleton_react_fastapi)
- [Flutter and Spring](https://github.com/maesi321/dev_container_skeleton_flutter_spring)

## Mental model
The repo consists of following parts:
- src: working directory
- .devcontainer: defintion of dev-container workflow
- docs: space for project documentation (general, ideas, etc)

The src is mounted via volume into the container. The container itself provides a development environment with the required dependency installed. 
When the dev container is started via VS Code the service itself needs to be started manually, the container self runs infinitly as long as IDE is running.

## Setup
- Docker installed -> [Docker homepage](https://www.docker.com/get-started/)
- (optional) grant Docker more resources to enable smooth development
- VS Code installed -> [VS Code homepage](https://code.visualstudio.com/)
- VS Code extension "Dev Containers" installed -> [Marketplace page](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)
- downloaded or cloned this repo

## How to start
- open this repo in VS Code
- run "Dev Containers: Reopen in Container"
![alt text](/docs/assets/image.png)
- the first opening takes a few minutes
- happy coding (the service working on needs to be started manually)