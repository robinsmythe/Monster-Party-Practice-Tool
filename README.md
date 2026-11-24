# Monster Party Practice Tool

## What is this?
This is an IPS patch that you can use to modify a ROM for the game Monster Party (NES). This IPS patch edits the game in order to add helpful features for practicing the game, and was mainly created to aid speedrunners.

## How do I use this?
You will need to acquire a Monster Party ROM, either from dumping the ROM from a genuine cartridge or by looking for it online from trusted sources.

Then, you can download the IPS Patch and patch it to the ROM. There are a few ways to do this:
### RomPatcher.js - [https://www.marcrobledo.com/RomPatcher.js/](url)
This is the easiest way, as you just visit this website and select your ROM and then the IPS patch. Then it will download the patched ROM.
### LunarIPS - [https://www.romhacking.net/utilities/240/](url)
If you are familiar with using IPS patches, you might have this program already. This is also a very simple and easy way to patch the ROM.

## I have the patched ROM, now what?
In order to play this ROM on an NES console, you will need to use a flash cartridge. These are unfortunately quite expensive, so it is a bit difficult to play on a console. The most popular flash cartridge is called the Everdrive N8, which can be found here:

### Cheaper Option - Everdrive N8
<ins>**Everdrive.me**</ins>  
NES Frontloader / USA Toploader [https://everdrive.me/cartridges/edn8nes72pin.html](url)  
Famicom / AV Famicom [https://everdrive.me/cartridges/edn8fami.html](url)

### More Expensive but more advanced option - Everdrive N8 Pro
<ins>**Krikzz.com**</ins>  
NES Frontloader / USA Toploader [https://krikzz.com/our-products/cartridges/everdrive-n8-pro-72pin.html](url)  
Famicom / AV Famicom [https://krikzz.com/our-products/cartridges/n8-pro-fami.html](url)

There are other flash cartridges out there, however I cannot speak to their quality. I have tested this ROM on my Everdrive N8, and it works fine.

If you own a flash cartridge, all you need to do is drag and drop the ROM onto the flash cartridge's SD card.

Now if you don't have a console or prefer to play on emulator, all you need to do is open the ROM in your preferred emulator! I used Mesen to create this patch.

## How to use this tool

### Video
[![Video Explanation](https://img.youtube.com/vi/_QZxxxNwCgA/0.jpg)](https://www.youtube.com/watch?v=_QZxxxNwCgA)

### Text Explanation
The controls for the menu are as follows:  
**L/R** to change the values  
**B** to change what you're selecting  
**START** when you are ready to start. Do not press onto Continue.    

<ins>**ROUND**</ins>  
This is what round you go into. You can select Round 1 to 9. (9 being the final boss)

<ins>**BOSS**</ins>  
This is what boss you want to spawn into. You pick 0 to just start the round as normal. In most rounds, you can pick 1, 2 or 3. In some Rounds, there are only two or less bosses.

<ins>**LIFE**</ins>  
This is defaulted at 12, which is what you typically start the game with. The minimum is 1 health, the maximum is 63 health.

<ins>**BERT**</ins>  
You can set this to either 0 or 1. 0 for Mark, 1 spawns you in as Bert. The power-up is not infinite, and will last as long as the normal power-up lasts.

<ins>**NEED**</ins>  
This is how many bosses you need to beat in order to get the Key. If you are just practicing an individual boss, this doesn't really matter. If you wanted to beat the game from a certain point, then you will have to change this accordingly. For example, if you wanted to play out the end of Round 1 from the 3rd Boss, you would set Need to 1. Then, when you beat Boss 3, you will get the Key. If you were starting from Round 1 Boss 1, you would set it to 3 and so on.

Round 7 is a special case, as you only need to beat 2 bosses in order to get the Key, however there are 3 bosses in the level. Keep in mind that if you beat all 3 bosses, it actually gives you the key on the 2nd boss and takes it away on the 3rd boss! So if you want to beat all 3 bosses in Round 7 and play the rest of the game out, set Need to 3. If you want to play Round 7 normally, just keep it at 2. It defaults to 2 on Round 7.

## Possible Questions and Probable Answers

### Why is part of the Monster Party logo cut off in the ROM? And why is the font different?
This is because I had to make space for more letters and numbers! There were not enough on the main menu to make a cohesive practice menu, so I opted to change some of the logo sprites in order to add more numbers. There were only 1, 9 and 8 by default thanks to the Bandai copyright year. You will be able to see the tiles I have changed when loading the ROM, and then they shortly get covered up when the edits kick in.

As to why the font is different, the main menu font is different to every other font used in the game - so if I added new sprites from elsewhere, it would have been mismatched. I thought it would just be easier and look better if it was all the same font.

### Why make this? This game has a password feature...
You are quite right. This game definitely doesn't NEED a tool like this, however I have always wanted to learn ASM and I thought this would be a good project to try. And hey, this game is cool.

### I picked Round 3 Boss 3 and it wasn't the boss I expected... why? WHY !!!
Unfortunately, I am just as confused as you are. The game has a peculiar boss order for certain Rounds, with Round 3 being completely backwards. In Round 3, the first boss you'd fight in the speedrun is the last boss in the boss list in the game code. It isn't like this for all levels however. To make things easier, I will list the boss numbers below. Next to the round number, I will include the the numbers of bosses that correspond with the speedrun. For example, Round 1 - 1 2 3 (as in Boss 1, 2 and 3 are in the right order.) and for Round 3 - 3 2 1 (as Boss 3 is the first Boss you'd beat in the speedrun).

<ins>**Round 1**</ins>   - 1 2 3  
Boss 1 - Eggplant  
Boss 2 - Dead Guy  
Boss 3 - Pumpkin Head  

<ins>**Round 2**</ins>   - 1 3 2   
Boss 1 - Medusa  
Boss 2 - Well  
Boss 3 - Onion Ring  

<ins>**Round 3**</ins>   - 3 2 1  
Boss 1 - Spider  
Boss 2 - Mummy  
Boss 3 - Minotaur  

<ins>**Round 4**</ins>   - 3 1 2  
Boss 1 - Cat  
Boss 2 - Music Dude  
Boss 3 - Samurai  

<ins>**Round 5**</ins>   - 1 2  
Boss 1 - Watch my dance!  
Boss 2 - Javelin  

<ins>**Round 6**</ins>   - 1  
Boss 1 - Faces  

<ins>**Round 7**</ins>   - 1 3  
Boss 1 - Royce  
Boss 2 - Demon  
Boss 3 - Spider II  

<ins>**Round 8**</ins>   - 1 3 2  
Boss 1 - Dragon (Watch out baby!)  
Boss 2 - Pharoah  
Boss 3 - Face My Wrath! (I am not sure what this is)  

<ins>**Round 9**</ins>   - 1  
Boss 1 - Nose  

### Could you complete a segmented run with this?
I don't see why not! I have made sure that the spawn points for the rounds match with where you spawn in the original game, and you should be able to complete the game from whichever point you choose. I did this in hopes that people can compare segment times with one another using the practice tool. Please let me know if you think there are points that don't line up properly, and I will look into it. Exiting the door after beating a boss spawns you back to where you were when you entered the door, however as you don't enter through the door when using the practice menu, I have just chose an appropriate point to spawn the player.


## Plans and Bug Fixes
### Things I hope to implement
- Infinite Bert Option
- Infinite Health Option
- Menu when pausing the game
- Boss timer (Possibility for ILs?)
- Maybe fix the boss order to how it is ordered in the speedrun?

### Known bugs
I have worked on this for quite a while now, however there are some slight bugs that I need to work on. I thought I'd release it now as it pretty much works fine, there are just some small issues. If you find any issues not listed here, please let me know by either reporting the issue on this github page, or by contacting me through speedrun.com (smythe) or discord (rsmythe).

-  Leaving Round 1 Boss 3 boss room will not use the changed colour palette that happens in Round 1
-  Dying and restarting the round messes up the amount of Bosses that need to be beaten to get the Key (however dying during a boss fight should work fine)
-  Continuing after death can just softlock you in certain scenarios.
