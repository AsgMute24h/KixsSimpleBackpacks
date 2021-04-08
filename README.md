# KixsSimpleBackpacks
Simple customizable, survival-friendly item backpack plugin

# Compatibility
- Spigot, Paper, & CraftBukkit on versions **1.13.x - 1.16.x** (other server types may work but are not directly supported)
- Java 8 or newer

![default backpack crafting recipe](https://i.imgur.com/2J5NR76.png)    ![backpack lore example](https://i.imgur.com/htdEMTS.png)

## Features
- **No dupes** unless the item is copied in creative mode; unique identifier assigned per backpack
- **Very customizable**; change backpack size, lore, display name, etc. (see [config.yml](src/config.yml))
- **No messy backend storage**; backpack contents stored in the item itself (PersistentDataContainer)
- **Anvil support** for renaming backpacks with respect to a configurable format
- **Rich meta**; backpack items show a summary of its contents along with slot usage and capacity in item lore
- **Dynamic config updates**; refreshes existing items in accordance to config changes:
  - If backpack size is made smaller, when players open their backpacks any items that previously fit in the older, bigger size will be dropped at their feet
  - Backpack item material, any text/lores from the config, and other options are refreshed and applied to backpacks when opened

## Commands & Permissions
- **/backpacks get**: get a backpack without having to craft it [permission: *backpacks.getcommand*]
- **/backpacks reload**: reload & update changes to the config file [permission: *backpacks.reload*]

## Compile
Requires Java 8 & Maven
