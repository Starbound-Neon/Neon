![Neon++cats3](https://user-images.githubusercontent.com/111540866/235280308-420053d0-1ebd-4be6-8bce-ffc498dbae2c.png)

# Neon++
## Utility DLL for Starbound - Client-side - Vanilla, StarExtensions(NOGUI) and Hasibound compatible

Neon++ is a dynamic-link library (DLL) that provides a set of functions for use in the game Starbound. It also has an ImGui interface version.
check out our [lua.md](https://github.com/Starbound-Neon/Neon/blob/main/Lua.md) for more info

### If you like this project, you can support the development of Neon++ here:
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/lonaasan)
<details><summary>
  
## Installation
  
</summary>
  
  ### Standalone
  
  Replacer method is currently unavailable because of Instability, please use an injector and inject Neon++ in the titlescreen.
  
  ### HasiboundLite
  
  DLL loading is planned in the future, for now, use the standalone way
  
  ### StarExtensions
  
  From the StarExtensions Github Site:
  >You can create a file called libraries.txt in the win64/win32 folder and list other DLLs to load on each line.

  If you, for example, put Neon++ into your win64 folder, you can write:\
  `Neon++.dll`\
  into the libraries.txt.

</details>
  
<details><summary>
  
## All functions:
  
</summary>
  
  All functions Neon++ provides. Look into [lua.md](https://github.com/Starbound-Neon/Neon/blob/main/Lua.md) for the documentation!

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

<details><summary>
  
## Demos:
  
</summary>

<details>
<summary><b>Change Difficulty</b></summary>
<br>
  
You messed up in your character creation and accidentally made it hardcore? Neon++ got your back with neon.player.setMode()!\
It lets you easily change your difficulty on the fly, so you can game on without making a new character!
</details>

<details>
<summary><b>Anti-grief & prevent malicious items</b></summary>
<br>
  
Your ship got raided? Other people on the server throw crashing items at you?\
Do not worry, Neon++ has options to protect your shipworld file and your inventory from malicious players!
</details>

<details>
<summary><b>Local Entity Destroy</b></summary>
<br>
Get rid of what you dont like! With Neon++ you can locally destroy entities.
<br>
<br>
  
![Neon_Local_Entity_Destroy](https://user-images.githubusercontent.com/111540866/235007493-9f8d77c3-c257-4f7b-9ce9-c8faf10c5fe1.gif)
</details>

<details>
<summary><b>Asset Spoofing</b></summary>
<br>
  
Tired of being locked from servers that dont allow you to use your fancy custom stuff? Neon++ got your back with asset spoofing!\
Just get the needed asset-digest from the logs and spoof it later with Neon++!
<br>
<br>
  
![Neon_Set_Asset_Digest](https://user-images.githubusercontent.com/111540866/235007533-bb019c40-ac98-42ae-b8d4-51bc289b8dc0.gif)
![Neon_Get_Asset_Digest](https://user-images.githubusercontent.com/111540866/235007537-068e9832-944e-4c6a-9935-fe398e6e53f3.gif)
</details>

<details>
<summary><b>Player UUID Spoofing</b></summary>
<br>
  
Spoof your UUID with Neon++! This provides some protection from unwanted visitors.\
(We will work on ways to make it even more protective!)
<br>
<br>

![Neon_Set_Player_UUID](https://user-images.githubusercontent.com/111540866/235007581-6786e028-b447-4209-b816-85a72c7cc594.gif)
</details>

<details>
<summary><b>Send Chat</b></summary>
<br>
Send your Messages with Neon++! You can also get the last message received.
<br>
<br>
  
![NVIDIA_Share_NJUsodI4hR](https://user-images.githubusercontent.com/111540866/235009671-065dcc8b-9884-464a-a630-66b648be0a70.png)
</details>
  
  and many more! Look in [lua.md](https://github.com/Starbound-Neon/Neon/blob/main/Lua.md) for all functions!
  
</details>
