# Lan Party Scripts

This repo is dedicated to how to run an LAN Party within your organization with minimal setup. I have included 
docker-compose scripts and minimal documentation on how to run reach one of them, including mod installs.

# Buying the games

If you want to buy the bundled games, you can choose the 
[Counter-Strike Complete](https://store.steampowered.com/bundle/236/CounterStrike_Complete/) on Steam that will already 
include both CS 1.6 and CS:Source. This is 

Minecraft can be bought on their [website](https://www.minecraft.net/en-us/store/minecraft-java-bedrock-edition-pc), and
you want to select the Java version (compatible with mods). You will probably also need to setup a custom launcher like
[Prism](https://prismlauncher.org/) to be able to select the matching game version. Alternatively, you can install 
it using one of the [unofficial launchers](https://github.com/fn2006/PollyMC) that will directly download the game 
without the hassle of Microsoft accounts or setting alternative launchers. **Java 21 is required to run the game, 
so [make sure install it](https://jdk.java.net/23/).**

Here are all the supported games:

## CS

Classical CS 1.6, configured with AMXMod for admin commands. Mod installation is manual.

## CS:Source

Source version of CS, configured with Metamod for admin commands.  Mod installation is manual.

## Minecraft

Minecraft server, configured with [BedWars plugin](https://github.com/ScreamingSandals/BedWars) and mod support. Mod 
installation is automatic.

## Agario

Simple open-source browser game based on the original [agar.io](https://agar.io/). It is not as fluid as the original
game but at least can be self-hosted. There are of course some bugs, but it is surprisingly fun if played in 5-10 
people.