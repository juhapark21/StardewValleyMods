# Gift Tastes Make (More) Sense
**Gift Tastes Make (More) Sense** is a Stardew Valley mod that adjusts some villager gift preferences to better match in-game context. 

## Installation
1. Install the latest version of SMAPI.
2. Install [this mod](https://www.nexusmods.com/stardewvalley/mods/35436) from Nexus mods.
3. Run the game using SMAPI. <br>
[The wiki](https://www.stardewvalleywiki.com/Modding:Player_Guide/Getting_Started) has a helpful guide on installation and troubleshooting if you need more help. 

## Configuration 
You can edit the [config.json](https://github.com/juhapark21/StardewValleyMods/blob/main/%5BCP%5D%20GiftTastesMakeSense/config.json) file to toggle each modified preference. <br>
Using [Generic Mod Config Menu](https://www.nexusmods.com/stardewvalley/mods/5098), you can configure the mod in-game by clicking the cog button on the title screen or by clicking "Mod Options" in the options menu in-game. 

## Compatibility 
Compatible with Stardew Valley 1.6+ on Linux/macOS/Windows. 

# Modified Preferences
Expand each preference for the rationale behind the change (may contain spoilers).
<details>
  <summary> Abigail likes jack-o-lanterns </summary>
  Secret note #1 mentions that Abigail loves the smell of carved pumpkin. 
</details>
<details>
  <summary> Abigail likes fairy stones </summary>
   Abigail likes purple, as well as the occult. Fairy stones are purple and are said to have been made from the bones of ancient fairies, as per an old miner's song. 
</details>
<details>
  <summary> Shane likes chicken statues </summary>
   Shane likes chickens. 
</details>
<details>
  <summary> Leah likes marble </summary>
   The item description says marble is "a very popular material for sculptures", and it is rarer/more expensive than other building materials. Leah spends each morning sculpting. 
</details>
<details>
  <summary> Lewis loves blueberries during summer </summary>
   On summer Sundays, Lewis comments that he enjoys fresh blueberries. 
</details>
<details>
  <summary> Shane likes Joja Cola after his 6-heart event </summary>
   Shane starts cutting down on alcohol after his 6-heart event, and he has been seen drinking Joja Cola instead (14-heart event). He also loves Joja Cola as a snack in the Movie Theater. 
</details>

### Why I made this project
I was sad and confused when I gifted Abigail a fairy stone in my first playthrough and she didn't like it. It's purple (she likes purple) and it's a mineral (she likes minerals)?? 

### What I struggled with 
- Game logic - making json files didn't seem like much coding at all, until I realized that my changes had to work with the game logic (ie villagers have a confusing gift-receiving algorithm) as well as the mod frameworks themselves (ie conditionals only work with the content patcher at specific spots in the file). Since gaps in how I thought a game mechanic works and the actual mechanic didn't show up as conventional error messages or crashes, it was harder to spot what I was doing wrong.  
- Since I wasn't using the features of a conventional "language" and moreso learning how to add to other people's code, there was little documentation, also making it harder. 

### What I learned 
- Test with every change <br>
  ...otherwise you might have to undo a lot of changes and re-implement them, one small feature at a time. 
- Don't assume that the same method will work for all variations of what I wanted to make <br> 
  Even small changes could mean it needs a completely different approach! 
- VSCode has really nice extensions <br>
  Text comparison and markdown preview extensions were amazing and saved me many open tabs 
