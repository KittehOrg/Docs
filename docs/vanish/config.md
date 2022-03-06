# Configuration

!!! tip

    For this documentation, if a value is listed as monkey.banana then it looks like

        monkey
            banana: value

### Fake announcement settings

These settings define things related to fake joining and quitting.

`fakeannounce.join`  
`fakeannounce.quit`

* Format for the message sent when a player fake joins or quits.
* Uses [MiniMessage](https://docs.adventure.kyori.net/minimessage/format.html) formatting.
* You can use `<player:name>` or `<player:displayname>` for built in inclusion of name or plugin-set display name.
* You can inject any placeholders using PlaceholderAPI
* Default values (matching the game's defaults):
    *   fakeannounce.join: `<yellow><player:name> joined the game.`
    *   fakeannounce.quit: `<yellow><player:name> joined the game.`

`fakeannounce.automaticforsilentjoin`

* If true, a player who joins without an announce message (see permissions) will automatically fake 
an announce on unvanishing
* Default value: `false`

### Plugin hooks

Set any of these to true to enable the hook. All are by default false.  
Other plugins are mentioned in this configuration, but they are always enabled as they do not change anything

`hooks.essentials`

*   Users with the right permissions node (see permissions) will be hidden in Essentials when vanished

`hooks.dynmap`

*   Vanished users will not be shown on the map
*   Users with a certain permissions node (see permissions) will ALWAYS be hidden.

`hooks.discordsrv`

*   Users fake joining / leaving will inform DiscordSRV if they have the correct permissions.

`hooks.squaremap`

*   Hidden players will not show up on squaremap.

### Other configuration options

`permissionsupdates.checkonworldchange`

*   If true, when a player changes world their vanish.vanish permission is checked and if false, player is set visible
*   Default value: false

`effects.lightning.count`

*   Sets the number of bolts to fire when a user with the lightning effect (See permissions) toggles visibility
*   Default value: 30

`double-sneak-during-vanish-switches-gamemode`

* This section enables a feature where a vanished player can double-tap the sneak key to switch to spectator or back. 
Convenient for moving through closed doors or walls.

### Debug and system options

These are settings you won't need to deal with unless getting help debugging

`debug`

*   Enables some debug output

`permtest`

*   Enables permissions testing command in-game
*   Command is /permtest permission.node or /permtest player permission.node
*   Requires permissions:
*   vanish.permtest.self for self testing (by default true for all)
*   vanish.permtest.other for testing other players (by default op only)

`configVersionDoNotTouch.SeriouslyThisWillEraseYourConfig`

* Used internally to track your config's version, in case value names are changed
* As the name says, just don't touch this. It will update itself.
* The number here does NOT refer to the version of VanishNoPacket
