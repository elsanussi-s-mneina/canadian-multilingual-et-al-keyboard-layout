# canadian-multilingual-et-al
I am trying to implement the Canadian Multilingual Standard Keyboard on MacOS or something as close as possible to the Standard.
I am trying to follow the keyboard layout at the web address http://kbdlayout.info/KBDCAN/ as a guide, and the picture at
https://upload.wikimedia.org/wikipedia/commons/5/55/KB_Canadian_Multilingual_Standard_comment-fr.svg

Note: due to the lack of a right control key on many keyboards, I have put the group 2 key as a dead key, option + shift + 2 (number row) .

## Understanding the structure of the Canadian Multilingual Standard Keyboard
- plain keys on the keyboard can type one of 5 characters.
  - group 1, level 1
  - group 1, level 2
  - group 1, level 3
  - group 2, level 1
  - group 2, level 2
  - (Never used in the standard: group 2, level 3)

Level 2 is supposed to be accessed by holding down the left or the right shift key, and then pressing the key in question.
Level 3 is supposed to be accessed by holding down the right control key, and then pressing the key in question.
Group 1 is accessed without any extra modifier keys pressed.
Group 2 is accessed by holding down the alt graph key (the right alt key on Windows keyboards)

## Where the Mac keyboards do not agree with the Standard
- Although MacOS keyboards do have a control key, they often lack a right control key on laptops especially.
- Even if they have both control keys, using a control key as a modifier key to type characters on MacOS often has strange unintended side effects, and doesn't work in all applications (that is my experience while trying to use the control keys here).
- MacOS treats both the left and right alt keys as option keys, effectively the same thing as alt graph keys. There is no distinction between left and right option keys in the Mac tradition.

## How I dealt with these differences.
Since the option key on the Mac is very similar to the alt graph key, I treated it as the alt graph key according to the standard.
As for control, and control+shift, I have decided to not use those key combinations and instead use option+2. The number 2 was chosen
to act as a quick mnemonic in order to access group 2. Otherwise, if you do so very often it is suggested you type option+shift+; (semicolon) as
it is easier to reach.


## Known constraints
1. Do not use any control key as a modifier key for typing characters.
   - It does not work on MacOS.
2. Keep option layer (the characters you can type while holding the option key (altgr on PC)) strictly according to the standard. No extra characters there.
3. Use option+shift for access to any non-standard functionality.
4. option+shift+2 will be used to access group 2.

## How to extend this keyboard layout
- This keyboard layout is designed to be extended for personal use. The way to do this is to add characters on the option+shift layer, and
to change the name of the keyboard layout slightly. You can fork this repository, and change on your own account if you want to share with
others.
- If you want to add many characters you can make a new group, and put the dead key on the number of the group you want to create. I am using group 3. You can replace group 

## My non-standard Extensions
# access to forward slash under option+shift+é
# About group 3: transliteration of Middle Eastern languages
- Although not standard, I wanted to type certain transliteration characters including dot under, and line under diacritics, and so I added a separate group, it is accessible at option + shift + 3 number row.


## Why did you make this keyboard layout:
1. I realized that the Canadian CSA keyboard layout that came with my Mac was not standard. It did not have access to group 2 in a reliable or discoverable manner by the keyboard viewer. Instead many of the keys were strewn around the option layer in a way reminescent of othe Apple keyboard layouts but only slightly similar to the standard.
2. Although the US International version is supposedly available on MacOS out of the box, it differs from the PC version available on Windows and is therefore not a good option for me.
3. Mac OS did not come with any attempt to implement the Canadian Multilingual Standard.
4. I have not found a keyboard layout for typing ISO-233, and so I decided to extend this one for now. 
