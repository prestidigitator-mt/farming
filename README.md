minetest mod Farming Redo
=========================

This mod improves all food and farming related content

Information
-----------

This mod must be named `farming` a simplified but improved version of the built-in farming
mod in minetest but with more foods, it comes with wheat, cotton, carrot, cucumber,
potato, melon, cotton, cocoa, corn, better pumpkin and tomato to start out with which
spawn throughout the map...

It also features that foods can be planted on tilled soil so for those then no seeds are required,
original wheat and cotton will require seeds which are found inside normal and jungle grass...

![screenshot.png](screenshot.png)

Tech information
----------------

Farming Redo is a simplified version of the built-in farming mod in minetest and comes with wheat, cotton, carrot, cucumber, potato and tomato to start out with which spawn throughout the map... new foods need only be planted on tilled soil so no seeds are required, original wheat and cotton will require seeds which are found inside normal and jungle grass...

This mod works by adding your new plant to the {growing=1} group and numbering the stages from _1 to as many stages as you like, but the underscore MUST be used only once in the node name to separate plant from stage number e.g.

* "farming:cotton_1"      through to   "farming:cotton_8"
* "farming:wheat_1"       through to   "farming:wheat_8"
* "farming:cucumber_1"    through to   "farming:cucumber_4"

https://forum.minetest.net/viewtopic.php?id=9019

Farming Redo also works with Bonemeal mod for quick growing crops and saplings which can
be found at https://notabug.org/TenPlus1/bonemeal

#### Dependencies

* default

Optional dependences:

* stairs
* intllib (only for older engines)
* lucky_block (adds 47 lucky blocks)
* toolranks

#### Configuration

It reads the configuration values from two places, `minetest.conf` and `farming.conf`, this last
must be at world path, if you have older place at mod path will be read but must be deprecated.


| Configuration        | type  | default | place file   |  Notes about                             |
| -------------------- | ----- | ------- | ------------ | ----------------------------------------- |
| time_speed           | float |    73   | minetest.conf | Speed to grow up the plants on engine (used as base for seed) |
| farming_stage_length | float |  160.0  | minetest.conf | Contains a value used for speed of crop growth in seconds |
| farming.rarety       | float |  0.002  | farming.conf | default rarety of crops on map (higher number = more crops) |
| farming.min_light    |  int  |    12   | farming.conf | default minimum and maximum light levels crops need to grow |
| farming.max_light    |  int  |    15   | farming.conf | default minimum and maximum light levels crops need to grow |
| farming.carrot       | float |  0.001  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.potato       | float |  0.001  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.tomato       | float |  0.001  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.cucumber     | float |  0.001  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.corn         | float |  0.001  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.coffee       | float |  0.001  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.melon        | float |  0.001  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.pumpkin      | float |  0.001  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.cocoa        |  bool |  true   | farming.conf | true or false only |
| farming.raspberry    | float |  0.001  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.blueberry    | float |  0.001  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.rhubarb      | float |  0.001  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.beans        | float |  0.001  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.grapes       | float |  0.001  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.barley       |  bool |  true   | farming.conf | true or false only |
| farming.chili        | float |  0.003  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.hemp         | float |  0.003  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.garlic       | float |  0.001  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.onion        | float |  0.001  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.pepper       | float |  0.002  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.pineapple    | float |  0.001  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.peas         | float |  0.001  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.beetroot     | float |  0.001  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.mint         | float |  0.005  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.cabbage      | float |  0.001  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.blackberry   | float |  0.002  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.lettuce      | float |  0.001  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.soy          | float |  0.001  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.vanilla      | float |  0.001  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.artichoke    | float |  0.001  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.parsley      | float |  0.002  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.sunflower    | float |  0.001  | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |
| farming.grains       |  bool |  true   | farming.conf | true or false only |
| farming.rice         |  bool |  true   | farming.conf | true to enable crop/food in-game and on mapgen set spawn rarety |

#### Nodes and food

This farming mod provides a large featured basic foods production of farming:

| Node name               | Description name      |
| ----------------------- | --------------------- |
| farming:salt            | Salt                  |
| farming:salt_crystal    | Salt crystal          |
| farming:rose_water      | Rose Water            |
| farming:glass_water     | Glass of Water        |
| farming:sugar           | Sugar                 |
| farming:caramel         | Caramel               |
| farming:turkish_delight | Turkish Delight       |
| farming:garlic_bread    | Garlic Bread          |
| farming:donut           | Donut                 |
| farming:donut_chocolate | Chocolate Donut       |
| farming:donut_apple     | Apple Donut           |
| farming:porridge        | Porridge              |
| farming:jaffa_cake      | Jaffa Cake            |
| farming:apple_pie       | Apple Pie             |
| farming:cactus_juice    | Cactus Juice          |
| farming:pasta           | Pasta                 |
| farming:spaghetti       | Spaghetti             |
| farming:bibimbap        | Bibimbap              |
| farming:burger          | Burger                |
| farming:salad           | Salad                 |
| farming:smoothie_berry  | Triple Berry Smoothie |
| farming:spanish_potatoes | Spanish Potatoes     |
| farming:potato_omelet   | Potato omelet         |
| farming:paella          | Paella                |
| farming:flan            | Vanilla Flan          |
| farming:cheese_vegan    | Vegan Cheese          |
| farming:onigiri         | Onirigi               |
| farming:gyoza           | Gyoza                 |
| farming:mochi           | Mochi                 |

#### Items tools

| node name               | Description           |
| ----------------------- | --------------------- |
| farming:scythe_mithril  | Mithril Scythe (Use to harvest and replant crops)        |
| farming:hoe_bomb        | Hoe Bomb (use or throw on grassy areas to hoe land) |
| farming:hoe_wood        | Wooden Hoe            |
| farming:hoe_stone       | Stone Hoe             |
| farming:hoe_steel       | Steel Hoe             |
| farming:hoe_bronze      | Bronze Hoe            |
| farming:hoe_mese        | Mese Hoe              |
| farming:hoe_diamond     | Diamond Hoe           |
| farming:bowl            | Wooden Bowl           |
| farming:saucepan        | Saucepan              |
| farming:pot             | Cooking Pot           |
| farming:baking_tray     | Baking Tray           |
| farming:skillet         | Skillet               |
| farming:mortar_pestle   | Mortar and Pestle     |
| farming:cutting_board   | Cutting Board         |
| farming:juicer          | Juicer                |
| farming:mixing_bowl     | Glass Mixing Bowl     |
| moreores:hoe_silver     | Silver Hoe            |
| moreores:hoe_mithril    | Mitril Hoe            |

#### Nodes and Aliasing

This mod is a direct replacement for the old Farming Plus mod and
replaces all of it's nodes and items with one's found within
Farming Redo.

#### AMB

There is one abm for new group `group:growing`.

### Changelog:

- NEXT - Now blueberries can make blue dye, tweak soil types to work better with older 0.4.x clients and add spanish translation (thx mckaygerhard), add trellis setting to registered_crops and fix pea and soy crop names (thx nixnoxus), add strawberries if ethereal mod not active
- 1.46 - Added min/max default light settings, added lettuce and blackberries with food items (thanks OgelGames), added soya, vanilla and sunflowers (thanks Felfa), added tofu, added salt crystals (thanks gorlock)
- 1.45 - Dirt and Hoes are more in line with default by using dry/wet/base, added cactus juice, added pasta, spaghetti, cabbage, korean bibimbap, code tidy
options, onion soup added (thanks edcrypt), Added apple pie, added wild cotton to savanna
- 1.44 - Added 'farming_stage_length' in mod settings for speed of crop growth, also thanks to TheDarkTiger for translation updates
- 1.43 - Scythe works on use instead of right-click, added seed=1 groups to actual seeds and seed=2 group for plantable food items.
- 1.42 - Soil needs water to be present within 3 blocks horizontally and 1 below to make wet soil, Jack 'o Lanterns now check protection, add chocolate block.
- 1.41 - Each crop has it's own spawn rate (can be changed in farming.conf)
- 1.40 - Added Mithril Scythe to quick harvest and replant crops on right-click.  Added Hoe's for MoreOres with Toolrank support.
- 1.39 - Added Rice, Rye and Oats thanks to Ademants Grains mod.  Added Jaffa Cake and multigrain bread.
- 1.38 - Pumpkin grows into block, use chopping board to cut into 4x slices, same with melon block, 2x2 slices makes a block, cocoa pods are no longer walkable
- 1.37 - Added custom 'growth_check(pos, nodename) function for crop nodes to use (check cocoa.lua for example)
- 1.36 - Added Beetroot, Beetroot Soup (6x beetroot, 1x bowl), fix register_plant() issue, add new recipes
- 1.35 - Deprecated bronze/mese/diamond hoe's, added hoe bomb and deprecated hoe's as lucky block prizes
- 1.34 - Added scarecrow Base (5x sticks in a cross shape)
- 1.33 - Added cooking utensils (wooden bowl, saucepan, cooking pot, baking tray, skillet, cutting board, mortar & pestle, juicer, glass mixing bowl) for easier food crafts.
- 1.32 - Added Pea plant (textures by Andrey01) - also added Wooden Bowl and Pea Soup crafts
- 1.31 - Added Pineapple which can be found growing in savannah areas (place pineapple in crafting to obtain 5x rings to eat and a top for re-planting), also Salt which is made from cooking a bucket of water, added food groups so it's more compatible with Ruben's food mods.
- 1.30 - Added Garlic, Pepper and Onions thanks to Grizzly Adam for sharing textures
- 1.29 - Updating functions so requires Minetest 0.4.16 and above to run
- 1.28 - Added chili peppers and bowl of chili, optimized code and fixed a few bugs, added porridge
- 1.27 - Added meshoptions to api and wheat plants, added farming.rarity setting to spawn more/less crops on map, have separate cotton/string items (4x cotton = 1x wool, 2x cotton = 2x string)
- 1.26 - Added support for [toolranks] mod when using hoe's
- 1.25 - Added check for farming.conf setting file to disable specific crops globally (inside mod folder) or world specific (inside world folder)
- 1.24 - Added Hemp which can be crafted into fibre, paper, string, rope and oil.
- 1.23 - Huge code tweak and tidy done and added barley seeds to be found in dry grass, barley can make flour for bread also.
- 1.22 - Added grape bushes at high climates which can be cultivated into grape vines using trellis (9 sticks).
- 1.21 - Added auto-refill code for planting crops (thanks crabman77), also fixed a few bugs
- 1.20b - Tidied code, made api compatible with new 0.4.13 changes and changed to soil texture overlays
- 1.20 - NEW growing routine added that allows crops to grow while player is away doing other things (thanks prestidigitator)
- 1.14 - Added Green Beans from Crops mod (thanks sofar), little bushels in the wild but need to be grown using beanpoles crafted with 4 sticks (2 either side)
- 1.13 - Fixed seed double-placement glitch.  Mapgen now uses 0.4.12+ for plant generation
- 1.12 - Player cannot place seeds in protected area, also growing speeds changed to match defaults
- 1.11 - Added Straw Bale, streamlined growing abm a little, fixed melon rotation bug with screwdriver
- 1.10 - Added Blueberry Bush and Blueberry Muffins, also Pumpkin/Melon easier to pick up, added check for unloaded map
- 1.09 - Corn now uses single nodes instead of 1 ontop of the other, Ethanol recipe is more expensive (requires 5 corn) and some code cleanup.
- 1.08 - Added Farming Plus compatibility, plus can be removed and no more missing nodes
- 1.07 - Added Rhubarb and Rhubarb Pie
- 1.06 - register_hoe and register_plant added for compatibility with default farming mod, although any plants registered will use farming redo to grow
- 1.05 - Added Raspberry Bushels and Raspberry Smoothie
- 1.04 - Added Donuts... normal, chocolate and apple... and a few code cleanups and now compatible with jungletree's from MoreTrees mod
- 1.03 - Bug fixes and more compatibility as drop-in replacement for built-in farming mod
- 1.02 - Added farming.mod string to help other mods identify which farming mod is running, if it returns "redo" then you're using this one, "" empty is built-in mod
- 1.01 - Crafting coffee or ethanol returns empty bucket/bottle, also Cocoa spawns a little rarer
- 1.0 - Added Cocoa which randomly grows on jungle tree's, pods give cocoa beans which can be used to farm more pods on a jungle trunk or make Cookies which have been added (or other treats)
- 0.9 - Added Pumpkin, Jack 'O Lantern, Pumpkin Slice and Sugar (a huge thanks to painterly.net for allowing me to use their textures)
- 0.8 - Added Watermelon and Melon Slice
- 0.7 - Added Coffee, Coffee Beans, Drinking Cup, Cold and Hot Cup of Coffee
- 0.6 - Added Corn, Corn on the Cob... Also reworked Abm
- 0.5 - Added Carrot, Cucumber, Potato (and Baked Potato), Tomato
- 0.4 - Checks for Protection, also performance changes
- 0.3 - Added Diamond and Mese hoe
- 0.2 - Fixed check for wet soil
- 0.1 - Fixed growing bug
- 0.0 - Initial release

### Lucky Blocks: 39
