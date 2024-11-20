# Installation

To start installation, simply start downloading game files with:

```bash
docker compose up -d
```

You can configure your server with password using the `config/csserver.cfg`. Alternatively, here is the 
[cheat sheet](https://txdv.github.io/cstrike-cvarlist/) with all commands allowed on your server configuration. If you
want to play the vanilla game, you don't have to update anything. When changing configs, restart server for them to 
take effect.

The folder for mod installation is `./datas/serverfiles/cstrike`.

# Mods

Once the files are downloaded and the server started, you can install basic mods. For example:

```bash
docker exec -it --user linuxgsm cs-server ./csserver mods-install
```

You want to execute this command to install all three basic mods. This command is not really interactive, so you have
to manually do:

- metamod
- amxmodx
- amxmodxcs

To set yourself as the admin, update the config under `config/admins.ini`.

# Maps

The next step is installing custom maps. You can look for them at [GameBanana](https://gamebanana.com/mods/cats/5474).
If you are in a hurry, a couple of recommendations:

### de_rats

Everyone is the size of a mouse, inside a big kitchen.

[![](https://gamebanana.com/mods/embeddables/97091?type=large)](https://gamebanana.com/mods/97091)

### fy_pool_day

Random weapons in a pool.

[![](https://gamebanana.com/mods/embeddables/86562?type=large)](https://gamebanana.com/mods/86562)

### awp_india

AWP only map where players shoot at each other from the other side of the map.

[![](https://gamebanana.com/mods/embeddables/87358?type=large)](https://gamebanana.com/mods/87358)

### 35hp_2

Knife only map where everyone is one hit away from dying.

[![](https://gamebanana.com/mods/embeddables/98510?type=large)](https://gamebanana.com/mods/98510)

### he_glass_2

You have glass under you, and fight with grenades. Last man standing wins.

[![](https://gamebanana.com/mods/embeddables/95240?type=large)](https://gamebanana.com/mods/95240)

### de_747

Classic map playing inside a Boing 747.

[![](https://gamebanana.com/mods/embeddables/82979?type=large)](https://gamebanana.com/mods/82979)
