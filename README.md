# Hypixel-Skyblock-Remake
This project is an attempt to recreate the game SkyBlock in the latest version of Minecraft and multiplayer, for up to 8 people. Everything that is in the main game, will be added in the remake!

This project uses only data packs and resource packs, giving everyone the resources needed to add their own addons like items, custom islands, mobs, stats and more!
Almost every feature will be purely customizable, either directly from a section of the SkyBlock Menu (accessible to all admins), or through your own datapacks.
This project uses only vanilla resources, so there will be some changes in both gameplay and design (for example menus are reduced to 3 rows instead of 6), and the original features that are purely designed to be multiplayer will have some changes to adapt them to 8 players, or to make them entirely singleplayer.


# INFO FOR DATAPACK MAKERS:

## MENUS
- ### Inventory Menu
creates a menu with a list of items/loot-tables from a storage
- #### Items
- #### Loot Tables
`data merge storage temp:menu_ui {temp:{storage:"(storage)",nbt:"(nbt)",path:".(path)",ui_type:(1-3),type:"(item/loot)",loot_path:"(path)/"}}`
`storage` source
`nbt` path from the storage
`path` additional path

## FUNCTION TAGS
function #menu:hotbar > replaces slot hotbar.8 with a custom menu item, (e.g Game Menu, SkyBlock Menu, Quiver), requires player tag "hotbar_override" to function
function #items:new_item > modifies new vanilla items nbt (used for item modifiers on vanilla items)
function #skyblock:base_player_stats > sets player base stats (used for custom stats)


- `function #skyblock:selectors/player` player selector, "ticking"
- `function #islands:main` custom island functions, "ticking"
- `function #skyblock:selectors/player/trigger` trigger functions, "ticking"
- `function #skyblock:selectors/player/cooldown` player cooldowns, "ticking"
