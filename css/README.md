# Installation

To start installation, start downloading game files with:

```bash
docker compose up -d
```

You can configure your server with password using the `config/cssserver.cfg`. Alternatively, here is the
[cheat sheet](https://basicer.com/halflife-2-cvar-list) with all commands allowed on your server configuration. If you
want to play the vanilla game, you don't have to update anything. When changing configs, restart the server for them to
take effect.

The folder for mod installation is `./datas/serverfiles/cstrike`.

# Mods

Once the files are downloaded and the server started, you can install basic mods. For example:

```bash
docker exec -it --user linuxgsm css-server ./cssserver mods-install
```

You want to execute this command to install all two basic mods. This command is not really interactive, so you have
to manually do:

- metamodsource
- sourcemod

To set yourself as the admin, update the config under `config/admins_simple.ini`. After that, you will be able to use 
the command `sm_admin` on the server, and use many different commands. Create a bind for easy access:

```
bind k sm_admin
```

## NoBlock

The NoBlock plugin makes sure players cannot collide with each other on the map. It's generally a good thing in
tight maps (like GunGame), where players can get stuck on the same spawn position.

NoBlock is also **a must** when are running surf or bhop.

- [Link to mod page](https://forums.alliedmods.net/showthread.php?t=91617?t=91617)
- [Direct download link](https://forums.alliedmods.net/attachment.php?attachmentid=74064&d=1285431495)

Here are some useful commands:

- `sm_noblock <0 or 1>`: Removes player vs. player collisions. (Default: 1)

## GunGame

GunGame is fun for CSS because they make the game much more dynamic and fun for everyone. For the GunGame itself:

- [Link to mod page](https://forums.alliedmods.net/showthread.php?t=93977)
- [Direct download link](https://forums.alliedmods.net/attachment.php?attachmentid=133712&d=1400696532)

Here are some useful commands:

- `gg_enable`: Turn on gungame and restart the game.
- `gg_disable`: Turn off gungame and restart the game.
- `gg_restart`: Restarts the whole game from the beginning.

And for the deathmatch plugin, so that you instantly respawn:

- [Link to mod page](http://forums.alliedmods.net/showthread.php?t=103242)
- [Direct download link](https://forums.alliedmods.net/attachment.php?attachmentid=108943&d=1346584450)

Here are some useful commands:

- `sm_ggdm_enable <0 or 1>`: Enable/disable deathmatch (default 1).
- `sm_ggdm_sp_enable <0 or 1>`: Enable/disable spawn protection (default 1).
- `sm_ggdm_sptime <number>`: Sets the amount of seconds users will be protected
from getting killed on their respawn (default 2).

# Maps

The next step is installing custom maps. You can look for them at [GameBanana](https://gamebanana.com/mods/cats/5535).
If you are in a hurry, a couple of recommendations:

### gg_aim_close2

Good map for GunGame.

[![](https://gamebanana.com/mods/embeddables/133579?type=large)](https://gamebanana.com/mods/133579)

### gg_simpsons_h1

Good map for GunGame.

[![](https://gamebanana.com/mods/embeddables/124110?type=large)](https://gamebanana.com/mods/124110)

### surf_beginner2

Beginner map for surf.

For this map, you want to make sure to execute the following commands as admin, on your console (see
[here for explanation](https://www.tobyscs.com/cs-surf-settings/)):

```
sm_cvar sv_accelerate 10
sm_cvar sv_airaccelerate 1000
```

[![](https://gamebanana.com/mods/embeddables/137722?type=large)](https://gamebanana.com/mods/137722)

### awp_india

AWP-only map where players shoot at each other from the other side of the map.

[![](https://gamebanana.com/mods/embeddables/118646?type=large)](https://gamebanana.com/mods/118646)