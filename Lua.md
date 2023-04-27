# Lua Functions
The following functions are supported in the Neon++ DLL:

<br/>

## neon

<br>
neon.build

Returns the build number of the application.

Example usage:

`sb.logInfo(neon.build) -- Prints the build number of the application`

neon.version

Returns the version string of the application.

Example usage:

`sb.logInfo(neon.version) -- Prints the version string of the application`

neon.name

Returns the name of the application.

Example usage:

`sb.logInfo(neon.name) -- Prints the name of the application`

neon.uniqueId

Returns the unique identifier of the application.

Example usage:

`sb.logInfo(neon.uniqueId) -- Prints the unique identifier of the application`

neon.reloadMods()

Reloads the application with the current set of mods.

Example usage:

`neon.reloadMods() -- Reloads the application with the current set of mods`

<br/>

## neon.gui

(only gui version of the dll)

<br>

neon.gui.openGui<br>
(currently always open)

Enables the GUI. 

Example usage:

`neon.gui.openGui() -- Enables the GUI`

<br>

## neon.world

<br>
neon.world.removeEntity(entityId) 

(no player entity or you will crash right now)

Removes the entity with the specified ID from the world.

entityId - The ID of the entity to remove.

Example usage:

`neon.world.removeEntity(123) -- Removes the entity with ID 123 from the world`

<br/>

## neon.spoof

<br>
neon.spoof.setPlayerUUID(uuid)

Sets the player's UUID to the specified value.

uuid - The UUID to set.

Example usage:

`neon.spoof.setPlayerUUID("123e4567-e89b-12d3-a456-426655440000") -- Sets the player's UUID`

neon.spoof.getPlayerUUID()

Returns the player's current UUID.

Example usage:

`local uuid = neon.spoof.getPlayerUUID() -- Gets the player's current spoofed UUID`

neon.spoof.setAssetDigest(digest)

Sets the asset digest to the specified value.

digest - The digest to set.

Example usage:

`neon.spoof.setAssetDigest("0123456789abcdef0123456789abcdef0123456789abcdef0123456789abcdef") -- Sets the asset digest`

neon.spoof.getAssetDigest()

Returns the current asset digest.

Example usage:

`local digest = neon.spoof.getAssetDigest() -- Gets the current asset digest`

<br/>

## neon.chat

<br>
neon.chat.sendMessage(message[, chatMode])

Sends a chat message to the server.

message - The message to send.
chatMode - The chat mode to use. Defaults to 0 (normal chat).

Example usage:

`neon.chat.sendMessage("Hello, world!") -- Sends a chat message`

neon.chat.lastMessage()

Returns the most recent chat message received.

Example usage:

```
local count, message = neon.chat.lastMessage() -- Gets the most recent chat message
sb.logInfo(message.Nick, message.Text) -- Prints the nickname and text of the message
```