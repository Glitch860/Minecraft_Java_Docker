# Minecraft_Java_Docker
How to deploy a Minecraft Java server using Docker compose

COMMENTS:
This Compose file uses the itzg/minecraft-server image from Docker Hub to create a container for the Minecraft Java Edition server. The container_name is set to "minecraft-java" for easy identification.

The container is configured to expose the default Minecraft Java Edition server port 25565 to the host machine using the ports configuration.

Several environment variables are set to configure the Minecraft Java Edition server, including EULA, MOTD, DIFFICULTY, GAMEMODE, PVP, LEVEL_TYPE, LEVEL_SEED, and ENABLE_COMMAND_BLOCK. These can be adjusted to match your desired server settings.

The volumes configuration is used to mount the host directory ./data as a volume in the container, which will be used to store the server data.

With this Compose file, you can start the Minecraft Java Edition server container using the command 
```
docker-compose up -d
```
