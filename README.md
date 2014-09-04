unity-launcher-toggle
=====================


Toggle unity launcher to auto-hide or always show depending on current focused window

### Tested on Ubuntu 14.04. Should work for 12.10 and higher.


This script is inspired by [this] (http://askubuntu.com/questions/519589/hide-the-unity-launcher-when-an-application-is-maximized) question.

If you want to hide the Unity Launcher while using some applications, and always show while using others this script is for you.
You can still show the Launcher like you would when the launcher is set to Autohide.

## Requirements

Works on Ubuntu 14.04. Should also work on Ubuntu 12.10 or higher

`xdotool` must be intstalled

    $ sudo apt-get install xdotool 

## Installation

[Download](https://github.com/c0rp-aubakirov/unity-launcher-toggle/archive/master.zip) or clone this repository to your home directory, in my case it is `/home/c0rp`.

Go to `System Settings / Keyboard / Shortcuts / Custom Shortcuts`.

Add new shortcut, where:

`Name:` **toggle_launcher**

`Command:` **/home/c0rp/unity-launcher-toggle/toggle**

Add some Shortcut for this script, for example <kbd>Shift</kbd> + <kbd>F11</kbd>.

Now run daemon from terminal:

    $ cd home/c0rp/unity-launcher-toggle/
    $ ./daemon start
    
After this you should be able to toggle Unity Launcher show/hide using your Shortcut.

Script will remember for which application to hide laucher, and for which to show.
