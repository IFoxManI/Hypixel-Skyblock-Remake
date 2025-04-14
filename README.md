# Hypixel-Skyblock-Remake
This project is an attempt to recreate the game SkyBlock in the latest version of Minecraft and multiplayer, for up to 8 people. Everything that is in the main game, will be added in the remake!

This project uses only data packs and resource packs, giving everyone the resources needed to add their own addons like items, custom islands, mobs, stats and more!
Almost every feature will be purely customizable, either directly from a section of the SkyBlock Menu (accessible to all admins), or through your own datapacks.
This project uses only vanilla resources, so there will be some changes in both gameplay and design (for example menus are reduced to 3 rows instead of 6), and the original features that are purely designed to be multiplayer will have some changes to adapt them to 8 players, or to make them entirely singleplayer.


# INFO FOR DATAPACK MAKERS:

## MENUS
- ### Menu Page Functions
  - `interact:{playsound:{name:"namespace",pitch:"0-2"}}`
  - `interact:{tellraw:{text:"text",selector:"selector"}}`
  - `interact:{go_back:1}` number can be greater than 1
  - `interact:{page_function:"change_page",page:"_page_"}` note: page path is saved in the menus data "data.menu.page"
  - `interact:{page_function:"close"}`
    

- ### Inventory Menu
creates a list of menus that contain a list of items/loot-tables saved in a storage

- `data merge storage temp:menu_ui {temp:{storage:"",nbt:"",path:"",ui_type:"1-3",type:"item/loot",loot_path:"path"}}`
  - `storage`
  - `nbt`
  - `path`
  - `ui_type`
    - 1 = 9x2
    - 2 = 7x2
    - 3 = 7x1
  - `item_modifier`
- function `function menu:inv_menu/main`

#### Items
storage `skyblock:temp` `[{id:"minecraft:diamond_sword",count:1},{id:"minecraft:stone",count:32},{id:"minecraft:golden_pickaxe",count:1},{id:"minecraft:diamond",count:12},{id:"minecraft:diamond",count:12},{id:"minecraft:diamond",count:12},{id:"minecraft:diamond",count:12},{id:"minecraft:diamond",count:12},{id:"minecraft:diamond",count:12},{id:"minecraft:diamond",count:12},{id:"minecraft:diamond",count:12}]`

#### Loot Tables


## FUNCTION TAGS
function #menu:hotbar > replaces slot hotbar.8 with a custom menu item, (e.g Game Menu, SkyBlock Menu, Quiver), requires player tag "hotbar_override" to function
function #items:new_item > modifies new vanilla items nbt (used for item modifiers on vanilla items)
function #skyblock:base_player_stats > sets player base stats (used for custom stats)


- `function #skyblock:selectors/player` player selector, "ticking"
- `function #islands:main` custom island functions, "ticking"
- `function #skyblock:selectors/player/trigger` trigger functions, "ticking"
- `function #skyblock:selectors/player/cooldown` player cooldowns, "ticking"
