# Spigot Plugin

## Development

Please use Intellij Idea to develop your mod or plugin. You can download it here: https://www.jetbrains.com/idea/download <br>
You have a Minecraft Development plugin for Intellij Idea. You can download it here: https://plugins.jetbrains.com/plugin/8327-minecraft-development (or search it on the plugins page of Intellij Idea)

> **Warning**
> Don't ask me how to use VsCode, I don't know 🤣

## Documentation
Wiki: https://www.spigotmc.org/wiki/spigot-plugin-development/ <br>
Scriptcraft Plugin (to write JS code): https://github.com/walterhiggins/ScriptCraft

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

## Tools

If you want to do some modeling you can use [BlockBench](https://www.blockbench.net/downloads). 

Plugins (Spigot):
- You can use [ModelEngine](https://www.spigotmc.org/resources/conxeptworks-model-engine-demo-1-16-5-1-19-3.106521/) to load bbmodel
- You can use [MythicsMobs](https://mythiccraft.io/index.php?pages/official-mythicmobs-download/&version=5.2.0) to create custom entities easily
- You can use [MythicsItems](https://mythiccraft.io/index.php?resources/crucible-create-unbelievable-mythic-items.2/) to create custom items with models

> **Warning**
> Check what type of model to use before starting ! <br>
> Plugins use Minecraft JSON or bbmodel (if you use ModelEngine plugin) <br>
