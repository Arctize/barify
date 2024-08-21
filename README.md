# barify

Adjust volume/brightness and display a bar using either dunst or mako.

## Example

Example using mako:

![image](img/example.png)

Using the following mako config (`~/config/mako/config`)

``` ini
layer=overlay
anchor=top-center
default-timeout=8000
border-size=2
background-color=#454545
progress-color=source #3b4d7e
border-color=#3b4d7e
border-radius=25
```

## Installation

* Place the script somewhere in your
  [PATH]((https://www.baeldung.com/linux/path-variable)) and make sure it's
  executable
* There's also an [AUR package](https://aur.archlinux.org/packages/barify).

Barify automatically uses either [mako](https://github.com/emersion/mako) or
[dunst](https://github.com/dunst-project/dunst), depending on which one it
detects.

## Usage

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
 