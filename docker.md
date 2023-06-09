**General Commands:**
- `docker --version`: Display the Docker version information.
- `docker info`: Display system-wide information about Docker.
- `docker help`: Display help information for Docker commands.

**Image Management:**
- `docker pull <image>`: Pull an image from a registry.
- `docker push <image>`: Push an image to a registry.
- `docker images`: List all images on the local system.
- `docker rmi <image>`: Remove an image from the local system.
- `docker build -t <image>:<tag> .`: Build an image from a Dockerfile in the current directory.
- `docker history <image>`: Show the history of an image.
- `docker tag <source_image>:<tag> <target_image>:<tag>`: Tag an image with a new name and/or tag.
- `docker save -o <file> <image>`: Save an image to a tar archive.
- `docker load -i <file>`: Load an image from a tar archive.
- `docker import <file> <repository>:<tag>`: Import the contents from a tarball to create a filesystem image.
- `docker export <container>`: Export a container's filesystem as a tar archive.

**Container Management:**
- `docker run -it --name <container_name> <image>`: Run a container interactively from an image.
- `docker run -d --name <container_name> <image>`: Run a container in detached mode (background).
- `docker ps`: List running containers.
- `docker ps -a`: List all containers, including stopped ones.
- `docker start <container>`: Start a stopped container.
- `docker stop <container>`: Stop a running container.
- `docker restart <container>`: Restart a container.
- `docker rm <container>`: Remove a container.
- `docker logs <container>`: View logs of a container.
- `docker exec -it <container> <command>`: Execute a command inside a running container.
- `docker cp <container>:<src_path> <dest_path>`: Copy files/folders between a container and the local filesystem.
- `docker commit <container> <image>:<tag>`: Create a new image from a container's changes.
- `docker attach <container>`: Attach local standard input, output, and error streams to a running container.
- `docker port <container>`: List port mappings or a specific mapping for the container.
- `docker top <container>`: Display the running processes of a container.
- `docker stats <container>`: Display a live stream of container(s) resource usage statistics.
- `docker pause <container>`: Pause all processes within a container.
- `docker unpause <container>`: Unpause all processes within a container.
- `docker wait <container>`: Block until a container stops, then print its exit code.
- `docker kill <container>`: Kill a running container using SIGKILL or a specified signal.
- `docker rename <old_name> <new_name>`: Rename a container.
- `docker update <container>`: Update configuration of one or more containers.

**Network Management:**
- `docker network create <network_name>`: Create a new network.
- `docker network ls`: List all networks.
- `docker network rm <network_name>`: Remove a network.
- `docker network connect <network_name> <container>`: Connect a container to a network.
- `docker network disconnect <network_name> <container>`: Disconnect a container from a network.
- `docker network inspect <network_name>`: Display detailed information on one or more networks.

**Volume Management:**
- `docker volume create <volume_name>`: Create a new volume.
- `docker volume ls`: List all volumes.
- `docker volume rm <volume_name>`: Remove a volume.
- `docker volume inspect <volume_name>`: Display detailed information on one or more volumes.
- `docker volume prune`: Remove all unused volumes.

**Swarm Management:**
- `docker swarm init`: Initialize a swarm.
- `docker swarm join`: Join a swarm as a worker node.
- `docker swarm leave`: Leave the swarm.
- `docker swarm update`: Update the swarm.
- `docker node ls`: List nodes in the swarm.
- `docker node rm`: Remove a node from the swarm.
- `docker node update`: Update a node.
- `docker service create`: Create a new service.
- `docker service ls`: List services.
- `docker service rm`: Remove a service.
- `docker service update`: Update a service.
- `docker service logs`: Fetch the logs of a service.
- `docker service ps`: List the tasks of a service.
- `docker service scale`: Scale one or multiple replicated services.
- `docker service rollback`: Rollback a service to its previous version.
- `docker stack deploy`: Deploy a new stack or update an existing stack.
- `docker stack ls`: List stacks.
- `docker stack rm`: Remove a stack.
- `docker stack ps`: List the tasks in the stack.
- `docker stack services`: List the services in the stack.

**Secret Management:**
- `docker secret create`: Create a secret.
- `docker secret ls`: List secrets.
- `docker secret rm`: Remove a secret.
- `docker secret inspect`: Display detailed information on one or more secrets.

**Config Management:**
- `docker config create`: Create a config.
- `docker config ls`: List configs.
- `docker config rm`: Remove a config.
- `docker config inspect`: Display detailed information on one or more configs.
