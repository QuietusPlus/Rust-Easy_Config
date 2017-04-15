- [Commands](#commands)
    - [Input](#input)
    - [Debug](#debug)
    - [Network](#network)
    - [Client](#client)

# Commands

Open the console _(Default: <kbd>F1</kbd>)_ to use these commands.

## Input

Command | Description | Example
------- | ------- | -------
`buttons.altlook` | |
`buttons.attack` | |
`buttons.attack2` | |
`buttons.attack3` | |
`buttons.backward` | |
`buttons.chat` | |
`buttons.console` | |
`buttons.duck` | |
`buttons.forward` | |
`buttons.inventory` | |
`buttons.invnext` | |
`buttons.invprev` | |
`buttons.jump` | |
`buttons.left` | |
`buttons.map` | |
`buttons.reload` | |
`buttons.right` | |
`buttons.slot1` | |
`buttons.slot2` | |
`buttons.slot3` | |
`buttons.slot4` | |
`buttons.slot5` | |
`buttons.slot6` | |
`buttons.slot7` | |
`buttons.slot8` | |
`buttons.sprint` | |
`buttons.use` | |
`buttons.voice` | |
`chat.add` | |
`chat.add2` | |
`chat.open` | |
`client.bugreporter` | Open the bug reporter interface _(see: `input.bind`)_ | `bind f9 "bugreporter"`
`client.consoletoggle` | Toggle console _(see: `input.bind`)_ | `bind f1 "toggleconsole"`
`input.bind` | Add new keybind | `bind w "+forward"` |
`input.clearbinds` | Remove all existing keybinds | `clearbinds` |
`inventory.toggle` | Toggle the inventory interface | `bind tab "inventory.toggle"`
`inventory.togglecrafting` | Toggle the crafting interface | `bind q "inventory.togglecrafting"`
`note.craft_add` | |
`note.craft_done` | |
`note.craft_start` | |
`note.inv` | |

## Debug

Command | Description | Example
------- | ------- | -------
`batching.print_renderers` | |
`batching.refresh_renderers` | |
`client.benchmark` | |
`client.fps` | Show current frames per second in console | `fps`
`client.ping` | Show current ping in console | `ping`
`commands.echo` | Print a message to console | `echo "Hello world!"`
`commands.find` | Search for console commands and variables | `find graphics` _Filter "graphics" related_<br>`find .` _All commands and variables_
`console.clear` | |
`console.copy` | |
`data.export` | |
`debug.debugcamera` | |
`debug.debugcamera_unfreeze` | |
`debug.lookingat` | |
`debug.lookingat_debug` | |
`debug.noclip` | Toggle noclip mode _(Admin only!)_ | `noclip`
`debug.printhead` | |
`debug.printinput` | |
`debug.printpos` | |
`debug.printrot` | |
`debug.renderinfo` | |
`dev.debugplayer` | |
`dev.headtrack` | |
`dev.sampling` | |
`entity.debug_lookat` | |
`entity.find_entity` | |
`entity.find_group` | |
`entity.find_id` | |
`entity.find_parent` | |
`global.cleanup` | |
`global.colliders` | Collider information |
`global.dump` | Dumps the following information into a folder:<br><ul><li>System information</li><li>List of root gameobjects</li><li>List of root objects</li><li>A full hierarchy of gameobjects including component count</li><li>List of connected players including network stats</li><li>List of all instanced Objects</li><li>List of all instanced ScriptableObjects</li></ul> |
`global.ent` | |
`global.error` | |
`global.objects` | |
`global.queue` | |
`global.status_cl` | |
`global.subscriptions` | |
`global.sysinfo` | Show system information _(same as `F1` > `Info`)_ |
`global.textures` | |
`global.version` | Game version information |
`global.warmup` | |
`client.report` | |
`client.sv` | |
`ddraw.arrow` | |
`ddraw.box` | |
`ddraw.line` | |
`ddraw.sphere` | |
`ddraw.text` | |
`demo.play` | |
`demo.record` | |
`demo.stop` | |
`demo.timedemo` | |
`layer.culling` | |
`layer.hide` | |
`layer.show` | |
`layer.toggle` | |
`music.info` | Print information about the current song, section, and intensity level to the console | `music.info`
`pool.clear_assets` | |
`pool.clear_memory` | |
`pool.clear_prefabs` | |
`pool.print_assets` | |
`pool.print_memory` | |
`pool.print_prefabs` | |
`pool.print_rigcache` | |
`profile.start` | |
`profile.stop` | |
`trackir.recenter` | |
`trackir.refresh` | |
`weather.report` | Display current weather information "Clouds, Fog, Wind, Rain percentage"
`world.monuments` | Display list of monuments and their location

## Network

Command | Description | Example
------- | ------- | -------
`client.connect` | Connect to specified server | `connect localhost:28015`
`client.disconnect` | Disconnect from current server | `disconnect`

## Client

Command | Description | Example
------- | ------- | -------
`gc.collect` | Garbage collect | `gc.collect`
`gc.unload` | Unload collected garbage from memory | `gc.unload`
`global.free` | Free all possible memory | `free`
`global.exec` | Execute a file located in "`Rust\cfg`" | `exec example.cfg`
`global.quit` | Close the game | `quit`
`global.readcfg` | Load configuration from disk | `readcfg`
`global.writecfg` | Save configuration to disk | `writecfg`
