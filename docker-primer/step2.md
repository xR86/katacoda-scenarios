
## Useful commands in Docker

## Docker control commands

Run a docker container for `node` image (if it hasn't been found locally, it will automatically `pull`):
`docker run -t node`{{execute}}

Start a previously instantiated container (run has been done before, that container is found in `docker ps -a`):
`docker run -t hello-world`{{execute}}
`docker start <name>`

Connect to a container (attach a bash to the docker instance and login):
`docker exec -it <name> bash`

Stop a currently active container (container is listed in `docker ps`):
`docker stop <name>`


## Wrappers for classic Linux commands

Check running containers:
`docker ps`{{execute}}

Check running processes in specific container:
`docker top <name>`

Forward sync - from host to guest:
`docker cp ./ <name>:/`

Backward sync - from guest to host:
`docker cp <name>:/<some_file> ./`
  

**The basics** of Docker (other than this): [zeroturnaround.com/rebellabs/docker-commands-and-best-practices-cheat-sheet/](https://zeroturnaround.com/rebellabs/docker-commands-and-best-practices-cheat-sheet/)  
**Slightly more than needed**, you can find more useful commands here: [github.com/wsargent/docker-cheat-sheet](https://github.com/wsargent/docker-cheat-sheet)
