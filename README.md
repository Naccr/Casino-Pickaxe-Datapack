🎰 Casino Pickaxe
Turn every mining trip into a game of chance!
✨ Features
Casino Pickaxe adds a unique tool to Minecraft (Forge 1.20.1) that changes the way you gather resources. When you break specific blocks with this pickaxe, you don't get the usual block drop. Instead, you get a random reward from a custom loot pool!
The Pickaxe: A durable tool capable of mining standard blocks.
The Gamble: Break a block, get a surprise! Will it be a Diamond, a Stick, or something from another mod?
Fully Configurable: Designed for Modpack Creators. You can define exactly which blocks trigger the effect and what items are dropped using standard Data Packs.

🛠️ How to Configure Manually
To customize the mod, you need to override the default Tag (for blocks) and Loot Table (for drops) in your Data Pack.
1. Define Breakable Blocks (The Tag)
Create a JSON file at this exact path:
data/casino_pickaxe/tags/blocks/custom_breakable_blocks.json
Use "replace": true if you want to remove the default blocks and only use your own list.
JSON
{
  "replace": true,
  "values": [
    "minecraft:stone",
    "minecraft:netherrack",
    "create:zinc_ore"
  ]
}


2. Define the Drops (The Loot Table)
Create a JSON file at this exact path:
data/casino_pickaxe/loot_tables/gameplay/randomdropspool.json
Note: The filename must be exactly randomdropspool.json (no underscores).
You can add any item (even from other mods) and assign weights to determine rarity.
JSON
{
  "pools": [
    {
      "rolls": 1,
      "entries": [
        {
          "type": "minecraft:item",
          "name": "minecraft:cobblestone",
          "weight": 80
        },
        {
          "type": "minecraft:item",
          "name": "minecraft:diamond",
          "weight": 1
        },
        {
          "type": "minecraft:item",
          "name": "minecraft:golden_apple",
          "weight": 5
        }
      ]
    }
  ]
}


3. Apply the Changes
Place your folder in .minecraft/saves/YourWorld/datapacks/.
Run the command /reload in-game.
Enjoy your custom casino experience!

📦 Modpacks
You are free to use this mod in any modpack, provided that you give credit (a link to this page).


---------------------------------------------------------------------------


If you enjoy my mods and want to support my work, feel free to buy me a coffee! Your support helps me keep creating.  https://ko-fi.com/tartuf59
