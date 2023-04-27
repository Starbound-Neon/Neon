Functions
The following functions are defined in the DLL:

neon

neon.build
Returns the build number of the application.

Example usage:

lua
sb.logInfo(neon.build()) -- Prints the build number of the application

neon.version
Returns the version string of the application.

Example usage:

lua
sb.logInfo(neon.version()) -- Prints the version string of the application

neon.name
Returns the name of the application.

Example usage:

lua
sb.logInfo(neon.name()) -- Prints the name of the application

neon.uniqueId
Returns the unique identifier of the application.

Example usage:

lua

sb.logInfo(neon.uniqueId()) -- Prints the unique identifier of the application

neon.reloadMods
Reloads the application with the current set of mods.

Example usage:

lua
neon.reloadMods() -- Reloads the application with the current set of mods

neon.gui

neon.gui.openGui
Enables the GUI.

Example usage:

lua
neon.gui.openGui() -- Enables the GUI

neon.world

neon.world.removeEntity(entityId)
Removes the entity with the specified ID from the world.

entityId - The ID of the entity to remove.
Example usage:

lua
neon.world.removeEntity(123) -- Removes the entity with ID 123 from the world

neon.spoof

neon.spoof.setPlayerUUID(uuid)
Sets the player's UUID to the specified value.

uuid - The UUID to set.
Example usage:

lua
neon.spoof.setPlayerUUID("123e4567-e89b-12d3-a456-426655440000") -- Sets the player's UUID

neon.spoof.getPlayerUUID()
Returns the player's current UUID.

Example usage:

lua
local uuid = neon.spoof.getPlayerUUID() -- Gets the player's current UUID

neon.spoof.setAssetDigest(digest)
Sets the asset digest to the specified value.

digest - The digest to set.
Example usage:

lua
Copy code
neon.spoof.setAssetDigest("0123456789abcdef0123456789abcdef0123456789abcdef0123456789abcdef") -- Sets the asset digest

neon.spoof.getAssetDigest()
Returns the current asset digest.

Example usage:

lua
local digest = neon.spoof.getAssetDigest() -- Gets the current asset digest

neon.chat

neon.chat.sendMessage(message[, chatMode])
Sends a chat message to the server.

message - The message to send.
chatMode - The chat mode to use. Defaults to 0 (normal chat).
Example usage:

lua
Copy code
neon.chat.sendMessage("Hello, world!") -- Sends a chat message
neon.chat.lastMessage()
Returns the most recent chat message received.

Example usage:

lua
Copy code
local message = neon.chat.lastMessage() -- Gets the most recent chat message
print(message.Nick, message.Text) -- Prints the nickname and text of the message
