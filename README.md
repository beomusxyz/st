# st

Beomus's fork of st, a simple terminal implementation for X.

## Configuring st

The configuration of st is done by editing either config.h/config.def.h
and (re)compiling the source code. It is good practice to back up your working build of st and apply patches/modifications to a copy before merging the two.
Also, modifying ```config.def.h``` instead of ```config.h``` is encouraged, as well as removing the generated ```config.h``` file before recompiling, as leaving it will cause st to use the leftover config.h from the last update, instead of generating a new one and applying the new patches. But i'm not your dad, so you can do what you want.

## Beomus's build

Just clone this repo and compile with the following command:
```
  $ make clean install
 ```
st should put it's binary in ```/usr/local/bin``` by default. if compiling it it doesn't work, you can run that command as root too, it's what i do.


## Patching in more features

You can find a treasure trove of excellent patches for st over at https://st.suckless.org/patches/
Credit for those patches goes to their respective authors.
I did not write any of the patches used in this fork. (Shit's complicated, and i'm not a
C wizard like the suckless devs or the Stanford/MIT gods.) But I intend to contribute when I have the skill and the time to.

## Patches

The following patches have been applied to this fork

- Alpha (for transperency/alpha)
- Blinking Cursor (self explanatory)
- Newterm (opening new terminal in same dir with keyboard shortcut)
- Delkey (for proper delete key behavior)
- Dracula Colour Scheme
- Scrollback (shift + pgup/pgdown for scroll)
	- Scrolback mouse (shift + mousewheel for scroll)



