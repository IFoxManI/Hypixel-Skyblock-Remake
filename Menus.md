## MENUS
- ### Menu Page Functions
  - `tellraw:{text:"",selector:""}`
    - text: `text format`
    - selector: `@$`
  - `go_back:` number can be greater than 1
  - `interact:{page_function:"change_page",page:"_page_"}` note: page path is saved in the menus data "data.menu.page"
  - `interact:{page_function:"close"}`
    

- ### Inventory Menu
creates a list of menus that contain a list of items/loot-tables saved in a storage

- `data merge storage temp:menu_ui {temp:{storage:"",nbt:"",path:"",ui_type:"1-3",type:"item/loot",loot_path:"path"}}`
  - `storage`
  - `nbt`
  - `path`
  - `ui_type`

       1               | 2               | 3
      :------------------:|:---------------------:|:----------------------:
      ![](images/inv_menu1.png) | ![](images/inv_menu2.png) | ![](images/inv_menu3.png) 
  - `item_modifier`
  - `function` ran with storage `temp:menu_ui`, to modify the slot use `$(menu_slot)`
- `function menu:inv_menu/main`

#### Items
```
storage > skyblock:temp [{id:"minecraft:diamond_sword",count:1},{id:"minecraft:stone",count:32},{id:"minecraft:golden_pickaxe",count:1},{id:"minecraft:diamond",count:12},{id:"minecraft:diamond",count:12},{id:"minecraft:diamond",count:12},{id:"minecraft:diamond",count:12},{id:"minecraft:diamond",count:12},{id:"minecraft:diamond",count:12},{id:"minecraft:diamond",count:12},{id:"minecraft:diamond",count:12}]
```

#### Loot Tables
