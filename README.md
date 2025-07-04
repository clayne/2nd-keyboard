# 2nd-keyboard
ALL of Taran's scripts - (not just for the 2nd keyboard.)

IF YOU ARE NEW TO AUTOHOTKEY, AND WANT TO USE IT FOR VIDEO EDITING, START BY WATCHING THIS FULLY COMPREHENSIVE TUTORIAL VIDEO I MADE:
https://www.youtube.com/watch?v=T3vG8U5RoFw

------------

I (was) the main video editor for Linus Media Group. We put out multiple videos every day, so I had to learn how to work quickly, without sacrificing quality.
These AutoHotKey scripts speed up my workflow significantly. (Mostly for Premiere Pro and Explorer)

I pioneered the use of a 2nd keyboard purely for macros, and later, the concept of "wrapping" keystrokes inside of other keystrokes, (ideally, the super-function keys (F13-F24)) as a means of massively multiplying the number of unique available keys.

------------

Adding a 2nd, independent keyboard is remarkably difficult, as Windows has no native support for distinguishing between multiple keyboards. There are many possible solutions, which vary greatly in difficulty, functionality, stability, and price. Here's a spreadsheet that breaks it all down for you. My preferred solution (QMK) might not be best for you:

https://docs.google.com/spreadsheets/d/18e6-OlUzc_1wbGvm9zqMOwtC4oysm6C7XMU1bOf8Nrc/edit?usp=sharing


#### So, to summarize, if you want to make your own macro keyboard, these are all the methods that I know of:
- Luamacros (unstable/buggy, no longer recommended) https://youtu.be/Arn8ExQ2Gjg
- Interception https://youtu.be/y3e_ri-vOIo and https://youtu.be/Hn18vv--sFY
- iCue (K55) https://www.youtube.com/watch?v=I9HYN6qA5CY
- Razer Synapse (Cyonosa Chroma) https://www.youtube.com/watch?v=1Cr2S0O--vc
- QMK (Hasu USB converter, my current solution.) https://youtu.be/GZEoss4XIgc


#### Other potential methods that I have not personally tested
- MacroMyKBD https://github.com/lal12/macroMyKBD
- 2key, which uses a Raspberry Pi https://github.com/Gum-Joe/2Keys/blob/v0.3.5/docs/SETUP.md
- An alternative to the Hasu USB converter: https://github.com/oschwartz10612/Scanner-Pro-MK3
- An alternative to LuaMacros:
https://github.com/VollRahm/NotEnoughHotkeys/
- An alternative to Interception, sort of: https://github.com/evilC/AutoHotInterception
- Mulitkeyboard https://mediachance.com/multikeyboard/ apparently has many problems. More info: https://twitter.com/iamnottani/status/1271530470052974595 and https://twitter.com/weirdoyt/status/1257282783044493312



If all of this just seems like a huge PITA, just buy a Stream Deck instead: https://youtu.be/vhPLhfP1b_s

NOTE: You do not need a 2nd keyboard to use AutoHotKey. Most poeple don't. By the time you need to add a 2nd keyboard, you should already be quite familiar with how AutoHotKey works. You can probably use your function keys for AHK macros, and if your main keyboard has dedicated macro keys, you can also use those. (Assign them to obscure shortcuts like CTRL SHIFT ALT F1, and then, in AutoHotKey, assign that key combo to whatever you want.)

Basically, don't just add a 2nd keyboard because you think it's cool! Make sure you actually need it, because you've run out of space on your main keyboard.

## My AHK scripts

IF YOU ARE NEW TO AUTOHOTKEY, start here:
https://autohotkey.com/docs/Tutorial.htm
https://www.youtube.com/watch?v=T3vG8U5RoFw

I know there's a lot of scripts in this repository. Look here to see what launches when I start my computer:
https://github.com/TaranVH/2nd-keyboard/blob/master/INFO_and_PROFILES/startup_folder_TARAN_Aug_2018.png

Some of the scripts are #include-d in other scripts. The MAIN script from which most others are run, is this one - so, you can start here: https://github.com/TaranVH/2nd-keyboard/blob/master/ALL_MULTIPLE_KEYBOARD_ASSIGNMENTS.ahk

Some scripts can stand entirely on their own, like this one: https://github.com/TaranVH/2nd-keyboard/blob/master/Taran's_Windows_Mods/Both_Accelerated_Scrolling_1.3_AND_Cursor_click_visualizer.ahk

To see most of these scripts in action during a real workday, check out my "World's Most Advanced Editing Tutorial" https://www.youtube.com/watch?v=O6ERELse_QY

All my custom Premiere, Photoshop, and After Effects keyboard shortcuts can be found here: https://github.com/TaranVH/2nd-keyboard/tree/master/Settings_and_shortcuts

Please note, I'm not a real programmer (in this lifetime.) My organization can be bad, and my code can be spaghetti-y. I have, however, done extensive commenting... so if you know how to code, it should be pretty easy to figure out what's going on.

Help with this repository is appreciated, but don't feel bad if I never officially merge your scripts. I can't trust anything that I haven't fully tested myself, or something with code that I don't recognise or understand. These are my real day-to-day working scripts, so I can't compromise them for anybody. 

Sometimes I put out tutorials on my personal channel: https://www.youtube.com/user/TaranVH/videos ...and sometimes I make "reverse tutorials" where I ask questions instead.

Twitter is probably the most effective method for you to contact me: https://twitter.com/TaranVH

You're free to use any of these scripts for yourself. Take what you need, modify it to your heart's content.

My most used, most useful, simplest script is this one: https://www.youtube.com/watch?v=OqyQABySV8k

2023 update: Since quitting LMG, I don't edit nearly as many videos as I used to, so I also haven't been updating my scripts as much. I certainly have not abandoned this repo, but if you want a version that uses Autohotkey 2.0 and is written far more like a real programmer would, I recommend you check this out: https://github.com/Tomshiii/ahk
I am always very happy when poeple take the things I've stared and build and improve upon them, and this is a great example.

-----

To see all my currently assigned scan codes and virual keys, take a look at this spreadsheet: https://docs.google.com/spreadsheets/d/1GSj0gKDxyWAecB3SIyEZ2ssPETZkkxn67gdIwL1zFUs/edit?usp=drive_web&ouid=107638578296445823789

-----

As of August 2018, I've changed the root directory from this:

**C:\Users\TaranWORK\Documents\GitHub\2nd-keyboard**

to this:

**C:\AHK\2nd-keyboard**

which is an enormous improvement, since users no longer have to change all the scattered instances of "TaranWORK" to their own username. Now, a huge amount of the scripts are turn-key, as long as you don't move anything or change any file paths.

This also means that the Corsair K95 and Stream Deck direct-launch scripts are ready to go immediately.

The only disadvantage is that these AHK scripts will be available to ALL users on a machine. If you share a computer, you may wish to move them under your user account after all.

Make sure to populate your startup folder with file shortcuts, to launch all the scripts you want as soon as the computer boots up. KEEP IN MIND that there are TWO startup folders - one for your user account, and one for ALL users. Here they are:

*C:\Users\[YOUR_USERNAME]\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup*
(You can open up this by typing "shell:startup" in the explorer bar.) 

*C:\ProgramData\Microsoft\Windows\Start Menu\Programs\StartUp*
(You can open up this by typing "shell:Common Startup" in the explorer bar.)

---

**Some interesting-looking related repositories**

This is the kind of next-level macro stuff I would do if I was a real programmer:
https://github.com/sebinside/HotkeylessAHK
https://github.com/sebinside/AHK2PremiereCEP
Explanatory video: https://www.twitch.tv/videos/628889342

https://github.com/TaranVH/2nd-keyboard/pull/27 (easier install of Interception, apparently.)

After Effects scripts from someone with 11 years After Effects experience who just discovered AHK:
https://github.com/ivycomb/AutoAfterEffects


More info on how to use Adobe CEP stuff:

https://www.youtube.com/channel/UCmq_t_-4GLFu_nYaEDDModw/videos

https://github.com/Adobe-CEP/Samples/blob/master/PProPanel/jsx/PPRO/Premiere.jsx


