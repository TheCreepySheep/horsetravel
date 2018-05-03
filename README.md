# What is HorseTravel?
HorseTravel is a fast-travel system for servers with a medieval RPG feel.
# What does it do?
The plugin provides a way for server owners to scatter TravelPoints across the map and players will be able to travel between those points on a horse. Each TravelPoint consists of two locations, a *station* and a *teleport*. *Stations* are basically the endpoints of a journey, where players get on and off the horses, while *teleports* are locations where the horse teleports to and from another location. 
# How to use?
1) Set up your TravelPoint locations. For each TravelPoint both *station* and *teleport* have to be in the same world or that point will not be loaded. 
```
horseSpeed: 1.5
travelpoints:
  spawn:
    station: world,-200,64,61
    teleport: world,-200,64,57
  someotherplace:
    station: world,-200,64,61
    teleport: world,-200,64,57
```
2) Set up player interaction. Currently HorseTravel is designed to only provide the function layer, while point selection was meant to be handled by other plugins, such as [BossShop](https://www.spigotmc.org/resources/bossshop-powerful-and-playerfriendly-chest-gui-shop-menu-plugin.222 "BossShop on Spigot") to provide a convenient way for owners to add their own conditions however they like.

3) Make your player-interaction use the command */horsetravel &lt;playerName&gt; &lt;originTravelPointID&gt; &lt;destinationTravelPointID&gt;*

4) Enjoy!
# Commands
*/reloadhorsetravel* - reloads config
Usage: Console / with perm *horsetravel.reload*

*/horsetravel* - initates travel
Params:
*&lt;playerName&gt;*
*&lt;originTravelPointID&gt;*
*&lt;destinationTravelPointID&gt;*
Usage: Console
Needs the player to have *horsetravel.use*

# Found bugs?
Please report them [here](https://github.com/TheCreepySheep/horsetravel/issues "Issue Tracker").

# Suggestions?
I'm always open to suggestions and constructive criticism. You can send suggestions as a PM or comment on the [Spigot resource page](https://www.spigotmc.org/resources/horsetravel-an-rpg-fast-travel.56360/).

# Planned features
- Configurable departure messages
- Configurable arrival messages
- Apply blindness for a smooth transition
- Multilanguage support maybe?
