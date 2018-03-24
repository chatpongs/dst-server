# Sharded Setup
> Start multiple servers connected to one world.

This setup configures two servers, one overworld and one
underworld (caves) which are connected through sinkholes.

In order to generate caves you need to provide a
leveldataoverride.lua script to configure world generation.
A good starting place is to create a DST server in game and
then copy over the leveldataoverride.lua created in the
local Klei folder for the shard.

# Console command
```
docker exec overworld dst-server console "c_announce('Hello everybody')"
docker exec overworld dst-server console "c_rollback(1)" # Rollback for 2 days
```

ref - http://dontstarve.wikia.com/wiki/Console/Don%27t_Starve_Together_Commands
