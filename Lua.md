# Lua Functions
The following functions are supported in the Neon++ DLL:
<details><summary>
  
### Table of contents:
  
</summary>
  
  neon\
  neon.build\
  neon.version\
  neon.name\
  neon.uniqueId\
  neon.reloadMods()\
  neon.warpAnimation(bool)\
  neon.gui\
  neon.gui.openGui()
  
  neon.world\
  neon.world.removeEntity(entityId)\
  neon.world.respawnInWorld(bool)\
  neon.world.reachEntities(bool)\
  neon.world.ignorePhysicsObjectCollisions(bool)\
  neon.world.ignoreProjectileCollisions(bool)\
  neon.world.ignoreVehicleCollisions(bool)
  
  neon.player\
  neon.player.ignoreItemPickup(bool)\
  neon.player.ignoreShipUpdate(bool)\
  neon.player.setName(name)\
  neon.player.setMode(mode)\
  neon.player.setHairDirectives(directives)\
  neon.player.setHairGroup(group)\
  neon.player.setHairType(type)\
  neon.player.setFacialHairDirectives(directives)\
  neon.player.setFacialHairGroup(group)\
  neon.player.setFacialHairType(type)\
  neon.player.setFacialMaskDirectives(directives)\
  neon.player.setFacialMaskGroup(group)\
  neon.player.setFacialMaskType(type)\
  neon.player.setBodyDirectives(directives)\
  neon.player.setEmoteDirectives(directives)
  
  neon.spoof\
  neon.spoof.setPlayerUUID(uuid)\
  neon.spoof.getPlayerUUID()\
  neon.spoof.setAssetDigest(digest)\
  neon.spoof.getAssetDigest()
  
  neon.chat\
  neon.chat.sendMessage(message, chatMode)\
  neon.chat.lastMessage()
</details>
    
#
<details><summary>
  
## neon
  
</summary>

### neon.build

#### Returns the build number of the application.

Example usage:

```lua
sb.logInfo(neon.build) -- Prints the build number of the application
```

### neon.version

#### Returns the version string of the application.

Example usage:

```lua
sb.logInfo(neon.version) -- Prints the version string of the application
```

### neon.name

#### Returns the name of the application.

Example usage:

```lua
sb.logInfo(neon.name) -- Prints the name of the application
```

### neon.uniqueId

#### Returns the unique identifier of the application.

Example usage:

```lua
sb.logInfo(neon.uniqueId) -- Prints the unique identifier of the application
```

### neon.reloadMods()

#### Reloads the application with the current set of mods.

Example usage:

```lua
neon.reloadMods() -- Reloads the application with the current set of mods
```

### neon.warpAnimation(bool)

#### Shows the warp animation in the titlescreen.

`bool : bool - true or false.`

Example usage:

```lua
neon.warpAnimation(true)
```
</details>

#

<details><summary>
  
## neon.gui
  
</summary>

(only gui version of the dll)

### neon.gui.openGui()
#### Enables the GUI. 

Example usage:

```lua
neon.gui.openGui() -- Enables the GUI
```
</details>

#

<details><summary>
  
## neon.world
  
</summary>

### neon.world.removeEntity(entityId) 

#### Removes the entity with the specified ID from the world locally.

`entityId : int - The ID of the entity to remove.`

Example usage:

```lua
neon.world.removeEntity(123) -- Removes the entity with ID 123 from the world
```
### neon.world.respawnInWorld(bool) 

#### Gives you the ability to automatically respawn on the current world.

`bool : bool - true or false.`

Example usage:

```lua
neon.world.respawnInWorld(true) -- Respawns you on the world after dying
```
### neon.world.reachEntities(bool) 

#### Allows you to reach through walls (radius still unaffected).

`bool : bool - true or false.`

Example usage:

```lua
neon.world.reachEntities(true) -- Enables Wall Reach
```
### neon.world.ignorePhysicsObjectCollisions(bool) 

#### Ignoring physics-object collisions for your world.

`bool : bool - true or false.`

Example usage:

```lua
neon.world.ignorePhysicsObjectCollisions(true)
```
### neon.world.ignoreProjectileCollisions(bool) 

#### Ignoring projectile collisions for your world.

`bool : bool - true or false.`

Example usage:

```lua
neon.world.ignoreProjectileCollisions(true)
```
### neon.world.ignoreVehicleCollisions(bool) 

#### Ignoring vehicle collisions for your world.

`bool : bool - true or false.`

Example usage:

```lua
neon.world.ignoreVehicleCollisions(true)
```

</details>

#

<details><summary>
  
## neon.player
  
</summary>

### neon.player.ignoreItemPickup(bool)

#### Ignoring dropped items (for crash protection, spam, etc...).

`bool : bool - true or false.`

Example usage:

```lua
neon.player.ignoreItemPickup(true)
```
### neon.player.ignoreShipUpdate(bool)

#### Ignoring updates sent to your ship (for crash protection, spam, etc...). This feature will still allow for the temporary altering of your ship, but will keep your shipworld protected in not saving the altered state. (this includes updates you do)

`bool : bool - true or false.`

Example usage:

```lua
neon.player.ignoreShipUpdate(true)
```
### neon.player.setName(name)

#### Sets the name of the Player.

`name : string`

Example usage:

```lua
neon.player.setName("example")
```
### neon.player.setMode(mode)

#### Sets the game difficulty for the player.

`mode : int - 0 (Casual), 1 (Survival).`

Example usage:

```lua
neon.player.setMode(0)
```
### neon.player.setHairDirectives(directives)

#### Sets the hair directives of the player.

`directives : string`

Example usage:

```lua
neon.player.setHairDirectives("?crop=0;0;2;2?multiply=0000?blendscreen=/ai/ai.png;")
```
### neon.player.setHairGroup(group)

#### Sets the hair group of the player.

`group : string`

Example usage:

```lua
neon.player.setHairGroup("hair")
```
### neon.player.setHairType(type)

#### Sets the hair type of the player.

`type : string`

Example usage:

```lua
neon.player.setHairType("1")
```
### neon.player.setFacialHairDirectives(directives)

#### Sets the facial hair directives of the player.

`directives : string`

Example usage:

```lua
neon.player.setFacialHairDirectives("?crop=0;0;2;2?multiply=0000?blendscreen=/ai/ai.png;")
```
### neon.player.setFacialHairGroup(group)

#### Sets the facial hair group of the player.

`group : string`

Example usage:

```lua
neon.player.setFacialHairGroup("")
```
### neon.player.setFacialHairType(type)

#### Sets the facial hair type of the player.

`type : string`

Example usage:

```lua
neon.player.setFacialHairType("")
```
### neon.player.setFacialMaskDirectives(directives)

#### Sets the facial mask directives of the player.

`directives : string`

Example usage:

```lua
neon.player.setFacialMaskDirectives("?crop=0;0;2;2?multiply=0000?blendscreen=/ai/ai.png;")
```
### neon.player.setFacialMaskGroup(group)

#### Sets the facial mask group of the player.

`group : string`

Example usage:

```lua
neon.player.setFacialMaskGroup("")
```
### neon.player.setFacialMaskType(type)

#### Sets the facial mask type of the player.

`type : string`

Example usage:

```lua
neon.player.setFacialMaskType("")
```
### neon.player.setBodyDirectives(directives)

#### Sets the body directives of the player.

`directives : string`

Example usage:

```lua
neon.player.setBodyDirectives("?crop=0;0;2;2?multiply=0000?blendscreen=/ai/ai.png;")
```
### neon.player.setEmoteDirectives(directives)

#### Sets the emote directives of the player.

`directives : string`

Example usage:

```lua
neon.player.setEmoteDirectives("?crop=0;0;2;2?multiply=0000?blendscreen=/ai/ai.png;")
```

</details>

#

<details><summary>
  
## neon.spoof
  
</summary>

### neon.spoof.setPlayerUUID(uuid)

#### Sets the player's UUID to the specified value.

`uuid : string - The UUID to set.`

Example usage:

```lua
neon.spoof.setPlayerUUID("123e4567-e89b-12d3-a456-426655440000")-- Sets the player's UUID
```
### neon.spoof.getPlayerUUID()

#### Returns the player's current UUID.

Example usage:

```lua
local uuid = neon.spoof.getPlayerUUID() -- Gets the player's current spoofed UUID
```
### neon.spoof.setAssetDigest(digest)

#### Sets the player's AssetDigest to the specified value.

`digest : string - The AssetDigest to set.`

Example usage:

```lua
neon.spoof.setAssetDigest("fffffffffffffffffffffffffffffffffff")-- Sets the player's AssetDigest
```
### neon.spoof.getAssetDigest()

#### Returns the player's current AssetDigest.

Example usage:

```lua
local digest = neon.spoof.getAssetDigest() -- Gets the player's current AssetDigest
```

</details>

#

<details><summary>
  
## neon.chat
  
</summary>
  
### neon.chat.sendMessage( message , chatMode )

#### Sends a chat message to the server.

`message : string - The message to send.`

`chatMode : int - The chat mode to use. Defaults to 0 (normal chat).`

Example usage:

```lua
neon.chat.sendMessage("Hello, world!") -- Sends a chat message
```
### neon.chat.lastMessage()

#### Returns the most recent chat message received.

Example usage:

```lua
local count, message = neon.chat.lastMessage() -- Gets the most recent chat message

sb.logInfo(message.Nick, message.Text) -- Prints the nickname and text of the message
```
