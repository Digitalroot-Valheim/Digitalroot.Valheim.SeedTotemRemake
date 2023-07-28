# Summary
This is a remake of <a href="https://www.nexusmods.com/valheim/mods/969">Seed Totem</a> by MarcoPogo  
 
Original Mod: [https://www.nexusmods.com/valheim/mods/969](https://www.nexusmods.com/valheim/mods/969)

**Code is a refactor.**

## License
Original source released under the <a href="https://github.com/MathiasDecrock/ValheimMods/blob/master/LICENSE" target="_blank">WTFPL license</a>. (July 28, 2023)  
Remake Version is released under: **GNU Affero General Public License v3.0**

## Seed Totem  
Place the totem using the Hammer (can be configured to move to the Cultivator instead).  
It costs:  
- 5 Fine Wood
- 5 Greydwarf Eyes
- 1 Surtling Core
- 1 Ancient Seed

Use a seed with the item hotkeys to restrict the totem to a single type of seed. It will always make sure that newly placed plants have enough room to grow, but it won't check to make sure that everything around it still has enough room to grow; a totem is not that clever. Limiting it to one type of seed solves this issue.  

The green glow fades when the totem runs out of seeds, letting you know to add more.  

Also works with trees!  

Hold the Use key to add all permitted seeds in Inventory.  

Give the totem a whack to harvest all ready plants in the area. (Does not work on trees)  

## Advanced Seed Totem  
Construct a modified seed totem that plants in a rectangular area with the Artisan Table.  
It costs:  
- 10 Fine Wood
- 10 Greydwarf Eyes
- 2  Surtling Core
- 1  Ancient Seed

The totem scans the Cultivator, anything that creates a **Plant** object is considered a "seed". This means it will include both "Carrot" & "Carrot Seeds" for example. Notably this does not include the Berry Bushes from <a href="https://www.nexusmods.com/valheim/mods/1042" target="_blank">Plant Everything.</a> These are Pickable objects instead, they skip the Plant stage, but are permanent, so it should be fine to place them yourself.  

### Dependencies
- <a href="https://valheim.thunderstore.io/package/denikson/BepInExPack_Valheim/"  target="_blank">BepInExPack Valheim</a>
- <a href="https://github.com/Valheim-Modding/Jotunn" target="_blank">Jotunn (JVL)</a>

### Installation (manual)
1. Download the latest release archive (zip) file.
1. Extract the archive into &lt;Steam Location&gt;\steamapps\common\Valheim\BepInEx\plugins

### Configuration  
Most values are configurable:  
﻿
#### Server config  
- **Dispersion radius**: Dispersion radius of the Seed Totem (default: 5)
- **Dispersion time**: Time (in seconds) between each dispersion (default: 10)
- **Space requirement margin**: Extra distance to make sure plants have enough space (default: 0.1)
- **Max retries**: Number of retries when randomly sampling possible planting locations(default: 8) (Don't increase too much, can cause lag!)
- **Max seeds in totem**: Soft limit of number of seeds (like the Kiln or Smelters), 0 is no limit (default: 0)
- **Dispersion count**: Maximum number of plants to place when dispersing (default: 5)
- **Harvest on hit**: Should the Seed totem send out a wave to pick all pickables in radius when damaged? (default: true)
- **Check for cultivated ground**: Should the Seed totem also check for cultivated land? (default: true)
- **Check for correct biome**: Should the Seed totem also check for the correct biome? (default: true)
- **Custom piece requirements**: Load custom piece requirements from seed-totem-custom-requirements.json instead of default? (default: false)

#### Local config (not enforced)   
##### UI  
- **Build menu**: In which build menu is the Seed totem located (default: Hammer)
- **Show queue**: Show the current queue on hover (default: true)

##### Graphical
- **Glow lines color**: Color of the glowing lines on the Seed Totem (default: green)
- **Glow light color**: Color of the light from the Seed totem (default: green)
- **Glow light intensity**: Intensity of the light from the Seed totem (default: 3)
- **Glow flare color**: Color of the light flare from the Seed totem (default: green)
- **Glow flare size**: Size of the light flare from the Seed totem (default: 3)

Issues/Bugs
Open an issue or bug on the <a href="https://github.com/Digitalroot-Valheim/Digitalroot.Valheim.SeedTotemRemak/issues" target="_blank">issue board﻿﻿.</a>

Questions
Ask a question on the <a href="https://github.com/Digitalroot-Valheim/Digitalroot.Valheim.SeedTotemRemak/discussions" target="_blank">discussions board﻿﻿.</a>

### Support Me @ https://www.buymeacoffee.com/digitalroot

<br /><br />
<br />
<p align="center">
<b>Digitalroot can be found in the Valhalla Legends Discord</b><br /><br />
  <a href="https://discord.gg/SsMW3rm67u" target="_blank"><img src="https://digitalroot.net/img/vl/vl_logo_125x154.png"></a>
</p>
