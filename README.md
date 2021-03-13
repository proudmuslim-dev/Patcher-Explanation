# Bug Fixes
- **Layers In Tab** - Fixes sometimes players not having a hat layer on tab. *default	
- **Parallax Fix** - Fix the camera being too far back, seemingly making your eyes be in the back of your head.
- **Culling Fix** - Fix false negatives in frustum Culling, creating sometimes invisible Chunks. (Can negatively impact performance)
- **Case Insensitive Commands** - Stop Vanilla commands from forcing case sensitivity. *default
- **Head Rotations** - Resolve an issue where your head would not properly rotate while riding an Entity. *default
- **Keep Shaders on Perspective change** - Keep Vanilla shaders you're currently using while also being able to toggle Perspective. *default
- **Resource Exploit Fix** - Fix an exploit in 1.8 allowing servers to look through directories. *default
- **Arrow Lighting** - Stop Arrows attached to an Entity from messing up Entity lighting.
- **Command Handling** - Fix Forge's command handler not Checking for a '/' at the start of a command. *default
- **Reset Death Timers** - Resolve an issue where changing the fullscreen state on the Game Over screen would lock the buttons. *default
- **Player Void Rendering** - Remove the black box around the player while in the void. *default
- **Fluid Stitching** - Fix missing edges in fluids. "Requires Chunk reload (F3+a)." (May cause Z-Fighting against blocks that aren't full size.) *default
- **Fullscreen Fix** - Resolve an issue where you could not maximize the game once toggling fullscreen. *default
- **Arm Rotations** - Resolve an issue where your arm rotation would be angled upwards when mounting an Entity. *default
- **Mouse Bind Fix** - Fixes an issue where keybinds bound to mouse buttons do not work in inventories. *default
- **Mouse Delay Fix** - Resolve an issue where your crosshair is a tick behind your head position. *default
# Performance
- **Disable Nametags Boxes** - Remove the transparent box around the nametag. 
- **Disable mapped Item frames** - Stop item frames only with maps as their item from rendering
- **Disable Item Frames** - stop item frames from rendering
- **Disable Semitransparent Players** - Stop semitransparent players from rendering.
- **Disable skulls** - Stop sakulls from rendering. 
- **Disable Armorstands** - Stop armorstands from rendering (Armorstands are commonly used for npc nametag rendering. enabling this will stop those from rendering as well.
- **Disable Enchantment Books** - Stop enchantment table books from rendering.
- **Disable Enchantment Glint** - Disable the enchantment glint on enchanted items/potions.
- **Disable Gl Error Checking** - Disable unnecessary constant checking for errors in OpenGL. (Requires restart once toggled.) *default
- **Disable End Portals** - Stop end portals from rendering.
- **Batch Model Rendering** - Render models in a single draw call, reducing the amount of OpenGL instructions performed a second. *default
- **Disable Mob Spawning** - Reduce memory usage by disabling the check for mob spawning despite the set game rule. (this will disable mob spawning in singleplayer)
- **Remove Cloud Transparency** - Remove transparency from clouds.
- **static Fog Color** - Simplify fog color creation with a static fog color. *default
- **Low Animation Tick** - Lowers the amount of animations that happen a second from 1000 to 500. *default
- **Instant World Swapping** - Remove the dirt screen and waiting time when switching a world. *default
- **Chunk Update Limit** - Specify the amount of updates that can happen a second.  
- **Particle Culling** - Stop particles that aren't visible to the player from rendering. *default
- **Static Particle Color** - Disable particle lighting checks each frame. *default
- **Entity Culling** - Stop entities that aren't visible to the player from rendering. *default
- **Entity Culling Interval** - The amount of time in ms between occlusion checks for entities. Shorter periods are more costly toward performance but provide the most accurate information. Lower values recommended in competitive environments.
- **Smart Entity Culling** - Stop entity culling effect when using OptiFine shaders. (Due to the way OptiFine shaders work, we are unable to make Entity Culling compatible at this time. *Default
- **Don't Cull Player Nametags** - Render nametags even when the player and nametag are occluded. 
- **Don't Cull Entity Nametags** - Render nametags even when the entity and nametag are occluded.
- **Don't Cull Armorstand Nametags** - Render nametags even when the armour stand is occluded.
- **Check Armorstand Rules** - Don't cull armorstands that have a marker set in their entity rules. This will result in a lot of unculled armorstands in places like Hypixel Skyblock, but will provide better entity visibility, while losing out on some performance improvements.
- **Optimized Font Renderer** - Use modern rendering techniques to improve font renderer performance. *default
- **Optimized Cloud Renderer** - Use modern rendering techniques to improve cloud renderer performance. *default
- **Optimized Item Renderer** - Cache information about items, avoiding recalculating everything about it every frame. *default
- **Optimized Resource Pack Discovery** - Optimize the time it takes to open the resource packs GUI. (Does not work with Labymod's RP24 addon.) *default
- **Downscale Pack Images** - Change all pack icons to 64x64 to reduce memory usage. *default
- **Disable Attached Arrows** - Stop arrows that are attached to a player from Rendering. 
- **Disable Moving Arrows** - Stop arrows that are airborne from rendering.
- **Disable Grounded Arrows** - Stop arrows that are in the ground from rendering.
- **Disable Shadowed Text** - Remove shadows from text. (can positively improve performance.)
- **Cache Font Data** - Cache font data allowing for it to be reused multiple times before needing recalculation. *default
- **Entity Render Distance Toggle** - Toggle allowing a custom entity render distance
- **Entity Render Distance** - Stop rendering entities outside of the specified radius
- **Disable Breaking Particles** - Remove block breaking particles for visibility.
- **Item Searching** - Stop items from searching for extra items to combine with when the stack is already full. *default
# Miscellaneous 
- **Remove Screen Bobbing** - While using View Bobbing, only remove the view aspect but have the hand still - bounce around.
- **Better Camera** - Stop blocks such as grass and tall plants from affecting your FOV as done in 1.14+. *default
- **Crosshair Perspective** - Remove the crosshair when in third person.
- **Better F1** - Hide nametags when in F1 mode.
- **Remove Ground Foliage** - Stop plants/flower from rendering. (Requires Chunk reload (F3+A).
- **Smooth Scroll-to-Zoom Animation** - Add a smooth animation when you scroll in and out while zoomed.
- **Smooth Zoom Animation** - Add a smooth animation when you zoom in and out.
- **Zoom Smooth Camera** - Remove the smooth camera effect when using zoom.
- **Zoom Sensitivity** - Use a custom mouse sensitivity when zoomed. this is a percentage of your normal sensitivity 
- **Smooth Zoom Function** - Change the smoothing function used in the smooth zooming animation.
- **Zoom Adjustment** - Scroll when using OptiFine's zoom to adjust the zoom level.
- **Toggle to Zoom** - Make OptiFine's zoom key a toggle instead of requiring you to hold it
- **Simplify FPS Counter** - Remove the additions OptiFine L5 and above makes to the debug screen fps counter. *default
- **Remove Water Overlay** - Remove the water texture overlay when underwater.
- **Show Own Nametag** - See your own nametag in third person.
- **Clean View** - Stop rendering your own potion effect particles.
- **Disable Text shadow** - Remove shadows from text. (Can positively impact performance).
- **Alternate Text Shadow** - Change the text shadow to only move down rather than moving to the side.
- **Add Text Shadow to Nametags** - Render nametag with shadowed text.
- **Numerical Enchantments** - Use readable numbers instead of roman numerals on enchants. *default
