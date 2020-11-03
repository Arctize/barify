# barify
Modify volume or brightness and display result as a bar via notifications (either dunst or mako).

### Installation
* Just throw the script somewhere and make sure it's in your $PATH.
* There's also an [AUR package](https://aur.archlinux.org/packages/barify).

Barify automatically uses either [mako](https://github.com/emersion/mako) or [dunst](https://github.com/dunst-project/dunst),
depending on which one it detects as running.

On mako, for now, barify simply kills existing notifications and places a new one, which is admittedly ugly.
This will be fixed as soon as mako supports replacing notifications by their IDs (e.g. https://github.com/emersion/mako/pull/270).

### Usage

    Usage: barify MODE ACTION
    Modify volume or brightness and indicate level as
    a bar via notifications (either dunst or mako).

     Example:

        barify vol up

     Arguments:
        MODE:
           Volume:     volume|vol|v
           Brightness: brightness|bright|b
        ACTION:
           Increase:   up|u|inc|i
           Decrease:   down|dec|d
           Mute:       mute|m
 
