# Swap-Characters-Between-Seasons-Part-1
The tutorial for you to swap characters between seasons for The Definitive Edition. This method was found by ClemyTheBest, BatuTH and GdaTyler, hope you'll have fun with this tutorial.

# Beginning
First, you'll need the materials if you want to make S3 work in S4 for example or S4 in S1. It's limited for now but hopefully in the future there will be more options.
[Here are the materials you need to download.](https://www.mediafire.com/file/sxgszrl6en70zsf/Materials_V2.rar/file)

You'll also need [ttarch](http://aluigi.altervista.org/papers/ttarchext.zip) to extract the files from ttarch files.
If you have the files then you are good to go for model swapping.

**CURRENT PROBLEMS:** Season 3 sadly doesn't work with any other season together, but it can work with any season by itself. Like if you plan to have Javier in S1, you'll have to have S3 characters otherwise everything will look invisible.

## STEP 1: Locate the ttarch files you need.
**Where can I find them?** It's real simple, just go to game's folder and you'll see a folder named Archives there. 

**Which files are necessary for model swapping?** If you just want to swap the characters and you don't care about facial animations then you'll need data.ttarch2 and txmesh.ttarch2.
The data.ttarch2 is needed for the skl (skeleton) of his character, otherwise the character can look bugged and the txmesh is for the character's meshes and textures.

**After finding the files, what do I do next?** And that's what the next step is for!

## STEP 2: Extracting the files.

**NOTE:** You'll have to do this method twice if you are planning to use S2 character in S3 for example. Because we'll need both seasons' files to be extracted.
For this step I'll be needing WDC_pc_WalkingDead202_data.ttarch2, WDC_pc_WalkingDead202_txmesh.ttarch2, WDC_pc_WalkingDead301_data.ttarch2, WDC_pc_WalkingDead301_txmesh.ttarch2

**What do we need those for?** I'll teach you to replace Javier with Alvin as a test.

But if you are planning to do otherwise, you can still follow those steps.


**DATA:**

You'll need to create a notepad and paste this, of course you have to edit it because I don't know where the game is in your computer. Don't forget to create a folder named data as well, copy it's location then paste it to inside of "C:\data". Don't delete the " though.

```
ttarchext.exe -k 96CA999F8DDA9A87D7CDD9BB93D1BEC0D79171DC9ED98DD0D18CD8C3A0B0C695C39C93BBCCCCA7D3B9D9D9D08E93BEDAAED18D77D5D3A3 0 "C:\(the game folder)\Archives\data.ttarch2" "C:\data"
```

Examples: WDC_pc_WalkingDead204_data.ttarch2, WDC_pc_WalkingDead305_data.ttarch2, WDC_pc_WalkingDead404_data.ttarch2


**TXMESH:**

You'll do the same method as you did for Data. Just rename the data.ttarch2 to txmesh.ttarch2

```
ttarchext.exe -k 96CA999F8DDA9A87D7CDD9BB93D1BEC0D79171DC9ED98DD0D18CD8C3A0B0C695C39C93BBCCCCA7D3B9D9D9D08E93BEDAAED18D77D5D3A3 0 "C:\(the game folder)\Archives\txmesh.ttarch2" "C:\data"
```

Examples: WDC_pc_WalkingDead204_txmesh.ttarch2, WDC_pc_WalkingDead305_txmesh.ttarch2, WDC_pc_WalkingDead404_txmesh.ttarch2

After copying, pasting and editing is done then save the notepad files as .bat and put them inside the ttarchext folder. Don't copy and paste all the codes together, seperate them! Because the program might not recognize what you are trying to do. Then open the .bat file and the rest will be done by the program.

## STEP 3: Renaming the necessary files.

**DATA:**
You'll need character skl file which can be found in data and meshes which can be found in txmesh.
For example I want Alvin to be Javier, right? Here's what you'll do:

You need to get Alvin's skeleton file from any season 2 episode, to make it easier his skeleton name is: sk54_alvin

Same goes for Javi, his skeleton name is: sk61_javier

You have to rename sk54_alvin to sk61_javier. After that we'll move to txmesh.

**TXMESH:**
S2 characters don't have many meshes but S3 characters do, and that's why we need to copy and paste Alvin's mesh and rename them as Javier's meshes.

Get sk54_alvin.d3dmesh from txmesh.ttarch2 and go to the other txmesh file you've extracted.

For example make a copy of Alvin's mesh lots of times and rename them to sk61_javier_hair, sk61_javier_head etc... Do it until you've replaced all of Javier's meshes.

After you are done with renaming Javier's meshes, get Alvin's textures which are d3dtx files (those are in txmesh.ttarch2 as well). Don't forget to copy them as well otherwise Alvin wouldn't have any texture, poor guy.


## STEP 4: Testing
After you are done with renaming the files and got the textures, put them into Archives folder. Also! Don't forget to use the materials, since I replaced Javier with Alvin I'll need to go to "S1, S2, Michonne, S4 to S3" folder and copy the files and put them into Archives.

Then open the game, to be sure go to character viewer choose A New Frontier (since I modded Javier) and if you see your character there then you did it! Now you can play as Alvin in The New Frontier.

## What will the next part of the tutorial include?
I'll tell you how to make their facial animations and mouth animations work, also another easy method to replace the characters but that is one of the buggiest methods and it might bug your game, it's optional though.
