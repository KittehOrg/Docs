# Commands

The commands listing on this page is broken into sections by purpose. Permission nodes required for a feature are listed. Note that these are not the only permission nodes in the plugin. See the Permissions page for that information.

### Vanishing


/vanish


*   Basic vanish toggle
*   If config _fakeannounce.automaticforsilentjoin_ is enabled, after a no-announce join there will be a fake announce here
*   Permission node: vanish.vanish
*   Alternate command: /v
*   Note: For all /vanish commands, can replace 'vanish' with 'v'

/vanish fakequit /vanish fakejoin

*   For fake quit, will ensure you are invisible and will fake an announcement unless already faked. Reverse for join.
*   To force a fake announcement, put 'force' after the command, and it will announce regardless.
*   Permission nodes: vanish.vanish, vanish.fakeannounce
*   Alternate command:
*   Can replace 'fakequit' with 'fq' and 'fakejoin' with fj.
*   Can replace 'force' with 'f'



/vanish on /vanish off

*   Set oneself visible or invisible. A toggle-free /vanish
*   Add 'fake' at the end to send a fake announcement.
*   This feature requires vanish.fakeannounce permission node

### Toggling Features

/vanish toggle

*   List features you can toggle
*   Command /vanish toggle <option>
    *   Toggles the option stated
    *   List of options:
        *   see - See vanished players
        *   nopickup - Block picking up dropped items
        *   nofollow - Block mobs from targeting you
        *   nointeract - Block any interactions
            *   Block breaking
            *   Block placing
            *   Pressure plates, buttons, other redstony things
            *   Hit things
        *   nohunger - Prevent losing hunger (or gaining!)
        *   nochat - Prevent chat
        *   chests - Silent chest opening (read only) and container opening
        *   damage-in - Block being hurt
        *   damage-out - Block hurting others
    *   Alternate command: Can replace 'toggle' with 't'
    *   Permission node: See permissions documentation for all toggle permissions



/vanish effects

*   List effects you can toggle
    *   Command /vanish effects <option>
    *   Toggles the option stated
    *   List of options:
        *   smoke
        *   explode
        *   lightning
        *   flames
        *   bats
            *   Number of bolts can be configured
*   Alternate command: Can replace 'effects' with 'e'
*   Permission node: See permissions documentation for all toggle permissions

### Management

/vanish check

*   Check your visibility



/vanish list

*   Get a list of vanished users
*   Permission node: vanish.list



/vanish reload

*   Reload most configuration options
*   Permission node: vanish.reload