- [Default client.cfg](#default-clientcfg)
- [Variables](#variables)
    - [Audio](#audio)
    - [Graphics](#graphics)
    - [Performance](#performance)
    - [Interface](#interface)
    - [Culling](#culling)
    - [Batching](#batching)
    - [Pooling](#pooling)
    - [Debug](#debug)
    - [Network](#network)
    - [Input](#input)
    - [Unsorted](#unsorted)

# Default client.cfg

```
audio.advancedocclusion "False"
audio.game "1"
audio.master "1"
audio.menumusicvolume "0.2"
audio.musicvolume "0.2"
audio.speakers "2"
audio.voices "1"
client.cambone ""
client.camdist "2"
client.camfov "70"
client.camoffset ""0.0, 1.0, 0.0""
client.lookatradius "0.2"
client.pushtotalk "True"
client.rockskin "0"
culling.entitymaxdist "5000"
culling.entityminanimatorculldist "30"
culling.entityminculldist "15"
culling.entityminshadowculldist "5"
culling.entityupdaterate "5"
culling.safemode "False"
decor.quality "100"
dev.netgraph "False"
effects.aa "1"
effects.ao "True"
effects.bloom "True"
effects.lensdirt "True"
effects.maxgibs "1000"
effects.motionblur "True"
effects.shafts "True"
effects.sharpen "True"
effects.vignet "True"
fps.limit "100"
global.assetwarmup "1"
global.censornudity "False"
global.god "False"
global.language "en"
global.perf "0"
global.prefabwarmup "1"
global.specnet "False"
global.streamermode "False"
graphics.af "1"
graphics.branding "True"
graphics.chat "True"
graphics.dof "False"
graphics.dof_aper "12"
graphics.dof_blur "1"
graphics.drawdistance "2500"
graphics.fov "75"
graphics.lso "False"
graphics.parallax "0"
graphics.revz "True"
graphics.shaderlod "600"
graphics.shadowcascades "1"
graphics.shadowdistance "100"
graphics.shadowlights "1"
graphics.shadowmode "2"
graphics.uiscale "1"
grass.displace "False"
grass.quality "100"
input.autocrouch "False"
input.flipy "False"
input.holdtime "0.2"
input.sensitivity "1"
mesh.quality "100"
nametags.enabled "True"
netgraph.enabled "False"
netgraph.updatespeed "5"
particle.quality "100"
playercull.enabled "True"
playercull.maxplayerdist "5000"
playercull.maxsleeperdist "30"
playercull.minculldist "20"
playercull.updaterate "5"
playercull.visquality "2"
terrain.atlasmipfix "True"
terrain.basetexcomp "True"
terrain.quality "100"
tree.quality "100"
voice.loopback "False"
water.quality "1"
water.reflections "1"
```

# Variables

Open the console _(Default: <kbd>F1</kbd>)_ to set these variables.

## Audio

Variable | Default | Value | Description
------- | ------- | ------- | -------
`audio.advancedocclusion` | `False` | `True` _Enabled_<br>`False` _Disabled_ | Use more advanced sound occlusion.
`audio.ambience` | `True` | `True` _Enabled_<br>`False` _Disabled_ | Ambience System.
`audio.framebudget` | `0.3` | | Max ms per frame to spend updating sounds.
`audio.game` | `1` | `0` ~ `1` | Volume: Game.
`audio.master` | `1` | `0` ~ `1` | Volume: Master.
`audio.menumusicvolume` | `0.2` | `0` ~ `1` | Volume: Main menu music.
`audio.musicvolume` | `0.2` | `0` ~ `1` | Volume: Music.
`audio.speakers` | `2` | `2` _Stereo_<br>`3` _4 speaker surround_<br>`4` _5 speaker surrround_<br>`5` 5.1 surround<br>`6` _7.1 surround_<br>`7` _Prologic_ | Speaker configuration.
`audio.voices` | `1` | `0` ~ `1` | Volume: Voices.
`hitnotify.notification_level` | `1` | `0` _Off_<br>`1` _Clientside (instant but small chance of false reports)_<br>`2` _Serverside (bit of a delay but always accurate)_ | Hit reporting.
`music.enabled` | `True` | `True` _Enabled_<br>`False` _Disabled_ | Enable music.
`music.songgapmax` | `480` | |
`music.songgapmin` | `240` | |
`voice.loopback` | `False` | `True` _Enabled_<br>`False` _Disabled_ |
`voice.ui_cut` | `0` | |
`voice.ui_lerp` | `0.2` | |
`voice.ui_samples` | `20` | |
`voice.ui_scale` | `1` |  | Increase or decrease interface size.
`client.pushtotalk` | `True` | `True` _Enabled_<br>`False` _Disabled_ | When enabled voice-chat will be in push-to-talk mode instead of always on.

## Graphics

Variable | Default | Value | Description
------- | ------- | ------- | -------
`aianimation.groundorient` | `True` | `True` _Enabled_<br>`False` _Disabled_ |
`aianimation.qualitydistance` | `100` | |
`aianimation.speedscale` | `True` | `True` _Enabled_<br>`False` _Disabled_ |
`effects.aa` | `1` | `0` _Off_<br>`1` _FXAA_<br>`2` _SMAA_<br>`3` _TSSAA_ | Anti-aliasing.
`effects.ao` | `True` | `True` _Enabled_<br>`False` _Disabled_ | Ambient occlusion.
`effects.bloom` | `True` | `True` _Enabled_<br>`False` _Disabled_ | High quality bloom.
`effects.footsteps` | `True` | `True` _Enabled_<br>`False` _Disabled_ | Footsteps.
`effects.lensdirt` | `True` | `True` _Enabled_<br>`False` _Disabled_ | Lens dirt.
`effects.maxgibs` | `1000` | `0` ~ `10000` | Max gibs _(maximum amount of broken objects when something get's destroyed)_.
`effects.motionblur` | `True` | `True` _Enabled_<br>`False` _Disabled_ | Motion blur.
`effects.shafts` | `True` | `True` _Enabled_<br>`False` _Disabled_ | Sun shafts.
`effects.sharpen` | `True` | `True` _Enabled_<br>`False` _Disabled_ | Sharpen.
`effects.vignet` | `True` | `True` _Enabled_<br>`False` _Disabled_ | Vignet.
`graphics.af` | `1` | `1` ~ `16` | Level of anisotropic filtering.
`graphics.dof` | `False` | `True` _Enabled_<br>`False` _Disabled_ | Depth of field.
`graphics.dof_aper` | `12` | |
`graphics.dof_blur` | `1` | |
`graphics.drawdistance` | `2500` | `500` ~ `2500` | Draw distance.
`graphics.fov` | `75` | `60` ~ `90` | Field of view.
`graphics.itemskins` | `True` | `True` _Enabled_<br>`False` _Disabled_ | Enable item skins.
`graphics.lodbias` | `0.5` | `0.25` ~ `5` | Level of detail distance. When set between 0 and 1 favors less detail. A setting of more than 1 favors greater detail.
`graphics.lso` | `False` | `True` _Enabled_<br>`False` _Disabled_ | Large scale occlusion.
`graphics.parallax` | `0` | `0` ~ `2` | Parallax mapping _(make textures appear to have more depth)_.
`graphics.quality` | `0` | `0` _Fastest (lowest texture resolution)_<br>`1` _Fast (low texture resolution)_<br>`2` _Simple (full texture resolution)_<br>`3` _Good_<br>`4` _Beautiful_<br>`5` _Fantastic_ | Graphics quality.
`graphics.revz` | `True` | `True` _Enabled_<br>`False` _Disabled_ | Reverse-Z _(reduces z-fighting / texture flickering)_.
`graphics.shaderlod` | `600` | `100` _Lowest details_<br>`200` _Detailed ground textures and rocks_<br>`300` _Detailed clothing_<br>`500` _Detailed trees and water_ | Shader level.
`graphics.shadowcascades` | `1` | `1` _None_<br>`2` _Two_<br>`4` _Four_ | A higher number of cascades gives better quality _(reduces shadow aliasing)_.
`graphics.shadowdistance` | `50` | `50` ~ `1000` | The maximum distance at which shadows will be visible. Shadows that fall beyond this distance will not be rendered.
`graphics.shadowlights` | `1` | `0` ~ `3` | Maximum dynamic shadows cast by light sources.
`graphics.shadowmode` | `2` | ~~`0` _Disabled_~~ _Shadows are now forced!_<br>`1` _Hard shadows_<br>`2` _Soft shadows (requires `graphics.quality` above `2`)_ | Determines which type of shadows should be used.
`grass.displace` | `False` | `True` _Enabled_<br>`False` _Disabled_ | Grass displacement.
`water.quality` | `1` | | Water quality.
`water.reflections` | `1` | | Water reflections.
`decor.quality` | `100` | `0` ~ `100` | Decor quality.
`grass.quality` | `100` | `0` ~ `100` | Grass quality.
`mesh.quality` | `100` | `0` ~ `200` | Object quality.
`particle.quality` | `100` | `0` ~ `100` | Particle quality.
`terrain.quality` | `100` | `0` ~ `100` | Terrain quality.
`tree.quality` | `100` | `0` ~ `200` | Tree quality.
`terrain.atlasmipfix` | `True` | `True` _Enabled_<br>`False` _Disabled_ |
`terrain.basetexcomp` | `True` | `True` _Enabled_<br>`False` _Disabled_ |

## Performance

Variable | Default | Value | Description
------- | ------- | ------- | -------
`decal.cache` | `False` | `True` _Enabled_<br>`False` _Disabled_ | Refresh every frame instead of only when marked as dirty.
`gc.interval` | `-1` | `-1` _Off_<br>`#` _Interval in seconds_ | Perform garbage collect and unload at a regular interval.
`global.assetwarmup` | `1` | `1` _Enabled_<br>`0` _Disabled_ | Asset warmup.
`global.prefabwarmup` | `1` | `1` _Enabled_<br>`0` _Disabled_ | Prefab warmup.
`global.maxthreads` | `8` | | Maximum amount of threads used.
`world.cache` | `True` | `True` _Enabled_<br>`False` _Disabled_ |

## Interface

Variable | Default | Value | Description
------- | ------- | ------- | -------
`graphics.branding` | `True` | `True` _Enabled_<br>`False` _Disabled_ | Branding _("`rust alpha`" overlay on the top-right)_.
`graphics.chat` | `True` | `True` _Enabled_<br>`False` _Disabled_ | Chat.
`graphics.hud` | `True` | `True` _Enabled_<br>`False` _Disabled_ | Enable HUD.
`graphics.uiscale` | `1` | `0.5` ~ `1` | Interface scale.
`chat.enabled` | `True` | `True` _Enabled_<br>`False` _Disabled_ | Enable or disable chat displaying.
`global.streamermode` | `False` | `True` _Enabled_<br>`False` _Disabled_ | Streamer mode.
`fps.limit` | `100` | | The maximum number of frames to render per second.
`global.language` | `en` | `af` `ar` `ca` `cs` `da` `de` `el` `en-PT` `en` `es-ES` `fi` `fr` `he` `hu` `it` `ja` `ko` `nl` `no` `pl` `pt-BR` `pt-PT` `ro` `ru` `sr` `sv-SE` `tr` `uk` `vi` `zh-CN` `zh-TW` | Language.
`global.perf` | `0` | `0` _Disabled_<br>`1` _+ Frames per second_<br>`2` _+ Latency_<br>`3` _+ Memory_<br>`4` _+ Garbage collect_<br>`5` _+ Ping_<br>`6` _+ Tasks_<br>`7` + Invokes | Performance overlay.
`nametags.enabled` | `True` | `True` _Enabled_<br>`False` _Disabled_ | Show player nametags.
`global.censornudity` | `False` | `True` _Enabled_<br>`False` _Disabled_ | Censor nudity.

## Culling

Culling avoids rendering something if the player cannot see it.

Variable | Default | Value | Description
------- | ------- | ------- | -------
`culling.debug` | `False` | `True` _Enabled_<br>`False` _Disabled_ |
`culling.entitymaxdist` | `5000` | | Maximum distance to show any players in meters.
`culling.entityminanimatorculldist` | `30` | | Minimum distance at which we start disabling animators for entities.
`culling.entityminculldist` | `15` | | Entity of any kind will always be visible closer than this.
`culling.entityminshadowculldist` | `5` | | Minimum distance at which we start disabling shadows for entities.
`culling.entityupdaterate` | `5` | | How many times per second to check for visiblity.
`culling.safemode` | `False` | `True` _Enabled_<br>`False` _Disabled_ | Culling safe mode; for debugging purposes only.
`culling.toggle` | `True` | `True` _Enabled_<br>`False` _Disabled_ | Enable/Disable occlusion culling.
`playercull.debug` | `False` | `True` _Enabled_<br>`False` _Disabled_ |
`playercull.enabled` | `True` | `True` _Enabled_<br>`False` _Disabled (always render, even when hidden)_ | Player culling _(disable if players are invisible)_.
`playercull.maxplayerdist` | `5000` | | Maximum distance to show any players in meters.
`playercull.maxsleeperdist` | `30` | | Maximum distance to show sleepers in meters.
`playercull.minculldist` | `20` | | Players of any kind will always be visible closer than this.
`playercull.updaterate` | `5` | | How many times per second to check for visiblity.
`playercull.visquality` | `2` | `0` _Chest_<br>`1` _Chest + Head_<br>`2` _Chest + Head + Arms_<br>`3` _Chest + Head + Arms + Feet_ | Quality of Vis.

## Batching

Batching is the process of combining multiple smaller objects into a single big object in order to make it faster to render.

Variable | Default | Value | Description
------- | ------- | ------- | -------
`batching.collider_capacity` | `30000` | |
`batching.collider_invalidate` | `True` | `True` _Enabled_<br>`False` _Disabled_ |
`batching.collider_submeshes` | `1` | |
`batching.collider_threading` | `True` | `True` _Enabled_<br>`False` _Disabled_ |
`batching.collider_vertices` | `1000` | |
`batching.colliders` | `True` | `True` _Enabled_<br>`False` _Disabled_ |
`batching.renderer_capacity` | `30000` | |
`batching.renderer_invalidate` | `True` | `True` _Enabled_<br>`False` _Disabled_ |
`batching.renderer_submeshes` | `1` | |
`batching.renderer_threading` | `True` | `True` _Enabled_<br>`False` _Disabled_ |
`batching.renderer_vertices` | `1000` | |
`batching.renderers` | `True` | `True` _Enabled_<br>`False` _Disabled_ |
`batching.verbose` | `0` | |

## Pooling

Variable | Default | Value | Description
------- | ------- | ------- | -------
`pool.chat` | `True` | `True` _Enabled_<br>`False` _Disabled_ |
`pool.conditional_models` `True` | | `True` _Enabled_<br>`False` _Disabled_ |
`pool.decor` | `True` | `True` _Enabled_<br>`False` _Disabled_ |
`pool.effects` | `True` | `True` _Enabled_<br>`False` _Disabled_ |
`pool.entities` | `True` | `True` _Enabled_<br>`False` _Disabled_ |
`pool.mode` | `2` | |
`pool.plants` | `True` | `True` _Enabled_<br>`False` _Disabled_ |
`pool.player_clothing` | `True` | `True` _Enabled_<br>`False` _Disabled_ |
`pool.player_collider` | `True` | `True` _Enabled_<br>`False` _Disabled_ |
`pool.player_model` | `True` | `True` _Enabled_<br>`False` _Disabled_ |
`pool.player_nametag` | `True` | `True` _Enabled_<br>`False` _Disabled_ |
`pool.renderer_batches` | `True` | `True` _Enabled_<br>`False` _Disabled_ |
`pool.skins` | `True` | `True` _Enabled_<br>`False` _Disabled_ |
`pool.sounds` | `True` | `True` _Enabled_<br>`False` _Disabled_ |
`pool.trees` | `True` | `True` _Enabled_<br>`False` _Disabled_ |

## Debug

Variable | Default | Value | Description
------- | ------- | ------- | -------
`fps.graph` | `0` | |
`global.timewarning` | `False` | `True` _Enabled_<br>`False` _Disabled_ | Show completion times in console.
`vis.attack` | `False` | `True` _Enabled_<br>`False` _Disabled_ | Turns on debug display of attacks.
`vis.protection` | `False` | `True` _Enabled_<br>`False` _Disabled_ | Turns on debug display of protection.
`dev.gender` | `-1` | |
`dev.netgraph` | `False` | `True` _Enabled_<br>`False` _Disabled_ |
`global.debugmode` | `False` | `True` _Enabled_<br>`False` _Disabled_ |
`global.developer` | `0` | |
`debug.ambientvolumes` | `True` | `True` _Enabled_<br>`False` _Disabled_ | Whether or not to update ambient light from environment volumes.
`debug.checktriggers` | `False` | `True` _Enabled_<br>`False` _Disabled_ | Debug triggers.
`debug.drawcolliders` | `False` | `True` _Enabled_<br>`False` _Disabled_ | Draw colliders.
`debug.skyreflection` | `False` | `True` _Enabled_<br>`False` _Disabled_ | Whether or not to update the sky reflection probe.
`global.god` | `False` | `True` _Enabled_<br>`False` _Disabled_ | If you're an admin this will enable god mode.
`net.debug` | `False` | `True` _Enabled_<br>`False` _Disabled_ |
`global.specnet` | `False` | `True` _Enabled_<br>`False` _Disabled_ | If enabled you will be networked when you're spectating. This means that you will hear audio chat, but also means that cheaters will potentially be able to detect you watching them.
`global.safemode` | `False` | `True` _Enabled_<br>`False` _Disabled_ |

## Network

Variable | Default | Value | Description
------- | ------- | ------- | -------
`lerp.enabled` | `True` | `True` _Enabled_<br>`False` _Disabled_ | Interpolation on network positions.
`lerp.smoothing` | `0.15` | `0` ~ `1` _Higher equals more smoothing_ | Post process smoothing.
`lerp.time` | `0.1` | `#` _Seconds (lower is more accurate, but also more jittery)_ | Seconds behind to lerp.
`netgraph.enabled` | `False` | `True` _Enabled_<br>`False` _Disabled_ |
`netgraph.updatespeed` | `5` | |

## Input

Variable | Default | Value | Description
------- | ------- | ------- | -------
`physics.minsteps` | `2` | `1` ~ `60` | The slowest physics steps will operate.
`physics.steps` | `32` | `10` ~ `60` | The amount of physics steps per second.
`input.autocrouch` | `False` | `True` _Enabled_<br>`False` _Disabled_ | Automatically crouch when needed.
`input.flipy` | `False` | `True` _Enabled_<br>`False` _Disabled_ | Inverted mouse y-axis.
`input.holdtime` | `0.2` | `#` | Amount of seconds USE should be held down for it to count as not just a press.
`input.sensitivity` | `1` | `#` | Mouse sensitivity.

## Unsorted

Variable | Default | Value | Description
------- | ------- | ------- | -------
`client.cambone` | ` ` | |
`client.camdist` | `2` | |
`client.camfov` | `70` | |
`client.camlerp` | `1` | |
`client.camoffset` | `(0.0, 1.0, 0.0)` | |
`client.camspeed` | `1` | |
`client.debugdragdrop` | `False` | `True` _Enabled_<br>`False` _Disabled_ |
`client.lookatradius` | `0.2` | | The radius of the sphere trace used to determine what you're looking at.
`client.maxreceivetime` | `20` | |
`client.maxunack` | `4` | | Max amount of unacknowledged messages before we assume we're congested.
`client.prediction` | `True` | `True` _Enabled_<br>`False` _Disabled_ |
`client.rockskin` | `0` | |
`demo.timescale` | `1` | |
`file.time` | `False` | `True` _Enabled_<br>`False` _Disabled_ |
