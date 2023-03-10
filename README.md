# Spigot Plugin

## Documentation
Wiki: https://www.spigotmc.org/wiki/spigot-plugin-development/

## Building

You can build your plugin using the `buildAndMove` gradle task or `build` and then move the jar to the plugins folder yourself. <br>
*The `buildAndMove` task will build the plugin and move it to the `server/plugins` folder.*

## Running

### Docker

You can run the server using `docker-compose up` <br>
The server content will be located in the `server` folder.

### Manually

To launch minecraft server, download: https://download.getbukkit.org/spigot/spigot-1.19.2.jar <br>
Create a new folder named `server` containing the `spigot-1.19.2.jar` file <br>
Create a `eula.txt` file with `eula=true` inside <br>
To launch the server, run `java -Xmx2048M -jar spigot-1.19.2.jar` (Xmx is the maximum memory allocated to the server) <br>
If you don't have a premium Minecraft account, don't forget to set `online-mode=false` in the `server.properties` file

Or run this
```bash
mkdir server && cd server
wget https://download.getbukkit.org/spigot/spigot-1.19.2.jar # or curl -LO https://download.getbukkit.org/spigot/spigot-1.19.2.jar
echo "eula=true" > eula.txt # Accept the eula
echo "online-mode=false" > server.properties # Only if you don't have a premium Minecraft account
java -Xmx2048M -jar spigot-1.19.2.jar 
```
