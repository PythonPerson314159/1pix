# 1pix Guide
### Welcome to 1pix!
Here's a quick guide on the game.

## Gameplay
### What is 1pix?
1pix is a rhythm game with a unique gimmick - your only graphic is a simple black or white pixel! Additionally, the game only requires a standard mouse to play - just left click, right click and scrolling.

### Gamemodes
1pix has five gamemodes that require you to interact with the pixel in different ways. 

1. clckr - Very simple. Click when the pixel is white, don't click when it's black.
2. scrlr - Similar to clckr, except you scroll down when it's white and scroll up when it's black.
3. swppr - Similar to clckr, except when on white, you alternate which mouse button you click from left to right and back again. The cycle always starts with right clicking. For a pattern of _black, white, black, white,_ your mouse inputs should be _right, rest, left, rest_.
4. spmmr - Same as swppr, but instead you alternate between spamming the mouse buttons and scrolling up and down on the scroll wheel as fast as you can (pattern starts on mouse spamming).
5. ctrlr - More complicated and isn't used that much, so it isn't necessary to fully get the hang of this one. Starting at a specified click speed (called the CPS floor), when the pixel is white, you increase your click speed (up to the "CPS cap"), and when it's black, you decrease it. Hard to get the hang of, but rewarding when you do.

### Indicators

In a 1pix map, there are two types of indicators - one for gamemode switching, and another for scoring (this one isn't necessary, though - more on that soon).

#### Gamemode indicator

For gamemode switching, there will be a 3 second run of black, followed by a certain number of white flashes, then a final 1.2 (ish) second stretch of black.

How do you discern a mode transition from this? The number of white flashes is the gamemode that's being switched to, in the same order as above! For example, one flash means you'll be switching to clckr, two flashes means you'll be going to scrlr, and so on.


#### Scoring indicator


For scoring, the game scores you in accuracy out of 100%. By default, this is directly shown during gamemode transitions and at the end of maps. However, if you're planning on playing this game in its purest form, you'll need to know this following info.

Just like the previous indicator, there will be a certain number of white flashes followed by a black rest. This will happen three times. Each of these bursts indicates a digit.

If you have nine white flashes, a break, four, a break, then two, your accuracy will be 94.2%. If you FC a map, however, you'll be shown a solid white flash for five seconds. Congrats!


### Play your first map

Head to the [Google Drive](https://drive.google.com/drive/folders/1LmvzV_VcLkiQBtmdXfcs4lx90PJPprWj) to download a map (below 2 stars, preferably). Download it, then go back to the [1pix homepage](https://1pix.netlify.app), click "upload map", and pick the one you just downloaded. Upon clicking "Play", you'll be taken to a page with some stats. You're shown:

- The map length
- The gamemode at the start, to avoid having to do a whole transition procedure at the beginning of each map
- The map's difficulty, from 0* to 11*, and from Extreme 1 to 4 (it's the mapper's opinion, though, so take it with a grain of salt)
- Your best accuracy on the map
- The number of times you've played the map
- The click window - if all of your inputs are within this time of perfection, you'll get a full combo. Otherwise, each click is scored on how accurate it is and averaged.
Song and artist

If you click the dropdown, you can get more technical info, like the song's BPM, or the exact times of the gamemode transitions.

Once you're ready, get your mouse out, click "Go", and enjoy playing through your very first 1pix map!


## Map Creation

### Setup

1pix offers you the ability to create your own maps. To get started, simply go to the homepage, click on "Create", and fill out the metadata needed. These things are:

- **Map name**
- **Map description**
- **Song** - you'll have to get an external link for these, as 1pix doesn't have servers. The easiest solution is to host it through Github (more info in the FAQ)
- **Song offset** - not needed, but if you want to start the song from a specific point that's not the beginning, you can play the song and click "Update" right when you want to start the song. You can also play it back to make sure the timing is right.
- **Song BPM** - simply listen to the song, tap along to the beat with a BPM counter, and type the number in there.
- **Starting gamemode**
- **Click window** - tighter windows (smaller number) will make the map's scoring stricter (and thus make the map harder), vice versa with more lenient windows.
- **CPS floor and cap** - you shouldn't need to change this, as the default values are pretty balanced. Additionally, your map will likely not even be affected by these number. Nonetheless, spmmr is only affected by the CPS cap, where if the player's click speed is at or above the cap, they get full points. For ctrlr, the CPS floor and cap act as bounds for the drifting CPS target - it will always be between those two numbers (or at one of them).
- **Difficulty** - you probably shouldn't be filling this out now, but after you've made some progress on your map, you can place your opinion on the map's difficulty. This game has a star system, from 0* to 11*, with the 12* category, Extreme, having four subtiers - Extreme 1 through Extreme 4 (keep in mind that these would be represented as 13 through 16 stars).

Once you're done, click create!

### Basic editor controls

The 1pix editor is where you create your levels. Unlike the gameplay, it's keyboard focused, with the main controls being:

#### Gameplay modification
- **Left arrow** - Add one beat to current run (of black or white)
- **Right arrow** - Remove one beat from current run
- **Up arrow** - Add 1/8 of a beat to current run
- **Down arrow** - Remove 1/8 of a beat from current run
- **Space** - New run (swap from black to white or from white to black)
- **Backspace** - Delete previous run (if you're deleting a run in the middle of a map, keep in mind that this will invert all future runs, this can be circumvented by clicking **Ctrl + Backspace**)
- **1 through 5** - Add a gamemode transition (1 is clckr, 2 is scrlr, 3 is swppr, 4 is spmmr, and 5 is ctrlr). Additionally, the game automatically sets the transition length to match with the song's beats so you never get off sync.
#### Playhead control
- **A** - Move playhead to previous run
- **D** - Move playhead to next run
- **P** - See a runthrough the map from the playhead (**Ctrl + P** to start from the beginning), it's not the actual gameplay (eg, no scoring) but just a preview
#### Quality of life
- **Scroll up/down** - Zoom in/out
- **Ctrl + scroll up/down** - Scroll left/right
- **Ctrl + Z** - Undo your last change (up to 25 changes can be reverted).
- **Ctrl + S** - Save map - even though there are occasional autosaves, you should still do this!

### Advanced editor controls
You can definitely build a maps only using the basic controls. However, you can also use these more advanced options:

- **Q** - Remove 100ms from current run
- **E** - Add 100ms to current run
- **Z** - Remove 10ms from current run
- **C** - Add 10ms to current run
- **X** - Remove 1ms from current run
- **W** - Add 1ms to current run
- **R** - Record inputs - release your mouse to leave a trail of black and hold down to make it white. The recording is inserted at the playhead, and you can choose to snap the beats to every eighth, fourth, half, or full beat. Once it's inserted, you can click Backspace to delete the entire recorded chunk.

You can change the metadata or download the level with the buttons on screen. Happy mapping!


## FAQ

### How do I upload songs to Github?

To do this, you have to

1. Download the song's mp3 file
2. Make a [Github](github.com) account
3. Create a repository
4. Click on "uploading an existing file" (bottom of page)
5. Upload the file
6. Commit the changes
7. Click on the file
8. Right click "Raw", and
9. Copy the link from there.

### I think my map is good, how do I get it on the Google Drive?

Simply download it and email the .1pix file to me [here](mailto:i.am.a.very.cool.person.29@gmail.com). I may shift the difficulty rating around a bit but your map should be up soon after sending.

---

### That's all you need to know to start playing 1pix. Have fun!
