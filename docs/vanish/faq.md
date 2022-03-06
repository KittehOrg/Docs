# Frequently Asked Questions

Below are a series of problems I see frequently come up from users, and their solutions.

### How do I disable lightning or explosions?

You have granted yourself (or your group) the permission node(s) for the(se) effect(s). 
Don't grant them, or negate them if you're granting a parent node. Consult the documentation
for your permissions plugin (I strongly recommend [LuckPerms](https://luckperms.net/)) for more info.

### When I leave, there's no quit message

You have granted yourself the vanish.silentquit node. This node disables all quit messages on you 
when you leave. Don't grant it or negate it if you're granting a parent node.

### I don't show up on dynmap! (With the dynmap hook enabled)

You have granted yourself the vanish.hooks.dynmap.alwayshidden node. Don't grant it or negate it 
if you're granting a parent node.

### How do I negate a permission node?

Check your permission plugin's documentation (I strongly recommend [LuckPerms](https://luckperms.net/)).
It's slightly different for each one.

### I don't use a permissions plugin

That's fine! But, you should really be using [LuckPerms](https://luckperms.net/). However, if you insist:

By default, ops get a very narrow range of permissions, but you can grant ops more permissions through [permissions.yml](http://wiki.bukkit.org/Permissions.yml).

### I didn't find a solution to my problem

Prompt help can be found on the [MOSS Discord](https://discord.gg/g4MNz2hgT7).  
Issues and Pull Requests can also be opened on [GitHub](https://github.com/mbax/VanishNoPacket).