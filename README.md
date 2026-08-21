Bingo Player TAS repository

CelesteTAS is a copy from [The CelesteTAS Github](http://github.com/VampireFlower/CelesteTAS)
The Grabless files are a copy from [The Grabless TASes done by euni and the challenges discord](https://github.com/EuniverseCat/miscCelesteTAS/tree/master/Grabless).
It should be noted, that these are true grabless files and not just variant grabless, so this project will change those a bit.
Pico8 Tases are a copy of [DemoJameson's port](https://github.com/DemoJameson/CelesteClassicTAS/tree/master) of the [Pico8 TASes](https://celesteclassic.github.io/tasdatabase/classic/)
The actual TASes were made by the Pico8 TASing community found [here](https://discord.gg/9Dm3NCS).


## The naming scheme for objective encoding file follows the following scheme:

### Chapter
like 1A, 2A, 3A.  
### Checkpoint
like start, shrine, chasm
for huge mess it also includes mess order
and for hollows the top or bottom route.  

### (optional) grabless  
### (optional) dashless
### (optional) heart and summit gems
### (optional) cassette 
### (optional) snowballs or oshiro stuns or seeker stuns or flags or orb or switch
### (optional) seeker kills
### (optional) keys
### (optional) bino
like 5bino or 4bino
### (optional) theo or misc cutscenes
like secret in 6A, reflection cutscene, diary in elevator shaft etc.
### (optional) berries
- arb (collects berries)
- progress (does not collect berries, only gets fast berries) (usually with a count, like 5progress)
- fast (collects berries)
- winged (gets the winged)
- seeded (gets the seeded)
- 1up, 2up, 3up (all included)

## Updating Maingame tas
This will notate the changes that need to be done, when updating the maingame tases to a newer version, since there are unfortunately things I changed in the maingame files for an easier time drafting the objectives.

### 1A
change the lvl_6 room to match this. This will only add a #top-hyper label, that is used in all 1A-crossing files
```
#lvl_6
  14,R,J
  15,U,Z
   1,L,J,G
   7,L
#top-hyper
  14,L,D,X
   1,R,J
  14,R,U,X
   4,R,J,G
   7,R
   5,R,J
   2,R,K,G
   5,R
  10,R,J,G
   9,R
   2,R,J
   7,R
  43
```

### 1SH0 and 1HC
add a frame of 1,F,180 to the lvl_s1 SNQ and add the #Exit label
```
27,L,D,X
  59,L,J
#Exit
   1,S
   1,F,180
   1,D
   1,J,F,180
SaveAndQuitReenter
  36

#Post Heart
```

### 2A
add a frame of 1,F,180 to the save and quit in awake, so #lvl_end_0

### 3A
add the #oshiro1 label to first huge mess visit
```
11,L,D,X
   1,R,K
   3,R,K,N
   1,S
   1,D,J
  34
#oshiro1
   2,R,K
   1,K
  14,R,U,X
   1,R,J,G
```
### 3SH, 3HC, 3SHC
3SH needs a oshiro1 label
all need another frame for SNQ
3HC needs a #Return label after Cassette
3SH needs a #Collect on heart
3SHC needs a #Return label after Cassette

### 4HC and 4SH0 need 1,F,180 like above
### 5B and 5S need the same at TTM and Unraveling
### 5HC needs that as well and a #Return at Cassette

### 7HC and 7SHC needs 1,F,180 on Heart

### Other changes
Go through the improvements and see if any of them would affect the current tases. This is the longest thing and there will be mistakes.
look for route diversions, since those are where different inputs matter