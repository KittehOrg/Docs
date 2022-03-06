# Permissions

There are three "group" permission nodes, that give a bunch of nodes.  

First, a list of those nodes. Then, parent nodes and lastly defining what every single node is.
I generally suggest you give staff `vanish.standard`

    vanish.standard:
        vanish.see  
        vanish.vanish
        vanish.list
        vanish.nopickup
        vanish.nofollow
        vanish.notrample
        vanish.nointeract
        vanish.nohunger
        vanish.fakeannounce
        vanish.preventdamage
        vanish.statusupdates
        vanish.adminalerts
        vanish.silentchests

    vanish.op: The nodes that ops get
        vanish.reload
        vanish.adminalerts
        vanish.permtest.all
        vanish.see
        vanish.vanish
        vanish.statusupdates
        vanish.list

    vanish.\*: Every node ever.
        vanish.standard
        vanish.nochat
        vanish.silentjoin
        vanish.silentquit
        vanish.toggle.all
        vanish.hooks.dynmap.alwayshidden
        vanish.hooks.essentials.hide
        vanish.permtest.all
        vanish.reload
        vanish.effects.smoke
        vanish.effects.explode
        vanish.effects.lightning
        vanish.effects.flames
        vanish.effects.bats
        vanish.effects.toggle.all


### Parent nodes

These nodes being true make the nodes listed under them true as well


    vanish.preventdamage:
        vanish.preventoutgoingdamage
        vanish.preventincomingdamage
    
    vanish.silentjoin:
        vanish.joinwithoutannounce
        vanish.joinvanished
    
    vanish.toggle.damage:
        vanish.toggle.damageout
        vanish.toggle.damagein
    
    vanish.toggle.all:
        vanish.toggle.silentchests
        vanish.toggle.see
        vanish.toggle.nopickup
        vanish.toggle.nofollow
        vanish.toggle.damage
        vanish.toggle.nointeract
        vanish.toggle.nochat
        vanish.toggle.nohunger
    
    vanish.effects.toggle.all:
        vanish.effects.toggle.smoke
        vanish.effects.toggle.explode
        vanish.effects.toggle.lightning
        vanish.effects.toggle.flames
        vanish.effects.toggle.bats


### All nodes

vanish.vanish - Vanish
vanish.vanish.on - Use /vanish on
vanish.vanish.off - Use /vanish off
vanish.see - See vanished players
vanish.statusupdates - Notification in chat about vanish status changes
vanish.list - Get a list of vanished users
vanish.fakeannounce - Fake joining and quitting
vanish.adminalerts - Receive alerts about updates
vanish.reload - Reload config stuffs

Vanish status effects:
vanish.nopickup - Block item pickups
vanish.nofollow - Block mob targeting
vanish.notrample - Block crop trampling
vanish.nointeract - Block placing/breaking/touching
vanish.nochat - Block chatting
vanish.nohunger - Block changing hunger level
vanish.preventincomingdamage - Prevent being hurt
vanish.preventoutgoingdamage - Prevent hurting others
vanish.preventdamage - Parent node to block all damaging
vanish.silentchests - Open chests read-only, no chest animation

vanish.joinwithoutannounce - Join the server without a "has joined"  
vanish.joinvanished - Join the server already vanished
vanish.silentjoin - Join vanished without announce
vanish.silentquit - Always (ALWAYS) leave the server without a
"has quit" message. ALWAYS.
If you want to not quit-message while vanished,
just do a fakequit when vanishing
Seriously think hard when assigning this node

Toggling. See above status effects:
vanish.toggle.nopickup
vanish.toggle.see
vanish.toggle.nofollow
vanish.toggle.notrample
vanish.toggle.nointeract
vanish.toggle.nochat
vanish.toggle.nohunger
vanish.toggle.silentchests
vanish.toggle.damagein
vanish.toggle.damageout
vanish.toggle.damage
vanish.toggle.all

Hooks features:
vanish.hooks.dynmap.alwayshidden - Be ALWAYS (ALWAYS) hidden on dynmap
vanish.hooks.essentials.hide - Hide in essentials
vanish.hooks.discordsrv.broadcastfakejoin - Broadcast fake joins to DiscordSRV
vanish.hooks.discordsrv.broadcastfakequit - Broadcast fake quits to DiscordSRV

Effects:
vanish.effects.smoke - Smoke effect on vanish toggle
vanish.effects.explode - Explosion effect on vanish toggle
vanish.effects.lightning - Lightning strike on vanish toggle

Effects toggling:
vanish.effects.toggle.smoke
vanish.effects.toggle.explode
vanish.effects.toggle.lightning
vanish.effects.toggle.all