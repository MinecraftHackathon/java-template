# Forge

## Development

Please use Intellij Idea to develop your mod or plugin. You can download it here: https://www.jetbrains.com/idea/download <br>
You have a Minecraft Development plugin for Intellij Idea. You can download it here: https://plugins.jetbrains.com/plugin/8327-minecraft-development (or search it on the plugins page of Intellij Idea)

> **Warning**
> Don't ask me how to use VsCode, I don't know 🤣

## Documentation

The official documentation is available at https://mcforge.readthedocs.io/en/1.19.2/gettingstarted/ <br>
French tutorials: https://www.minecraftforgefrance.fr/topic/12/sommaire-des-tutoriels <br>
KubeJS Mod (to write JS code): https://kubejs.com/, https://mods.latvian.dev/books/kubejs

## Running

Just run the `runClient` or `runServer` configuration of Intellij <br>
If you don't have any configuration (in the right upper corner), you can run `./gradlew genIntellijRuns` to generate them. <br>
If you want to use the gradle tasks directly, you can run `./gradlew runClient` or `./gradlew runServer` <br>

## Tools
If you want to do some modeling you can use [BlockBench](https://www.blockbench.net/downloads). 

Mod (Forge):
- You can use [GeckoLib](https://www.curseforge.com/minecraft/mc-mods/geckolib) to animate models
- You can use [ObjLoader](https://docs.minecraftforge.net/en/1.19.2/rendering/modelloaders/) to load obj models

> **Warning**
> Check what type of model to use before starting ! <br>
> Mod can use Minecraft JSON or OBJ model
