# mpd-scripts
Small collection of scripts for controlling MPD, usually using mpc.
Note: All desktop notifications are set to replace each other. This means that, for example, spamming the `mpd-playpause` script will NOT flood your screen with notifications.

## mpd-next
Uses mpc to skip to the next song.
Calls the `songinfo` script to display the information of the next song in the form of a desktop notification. You will probably need to change the path to the songinfo script.

## mpd-playpause
Uses mpc to toggle playback. Sends a notification with the action performed.

![image](https://github.com/allylikesu/mpd-scripts/assets/100547506/16477f5d-aa62-4076-8c87-d2af2d8c0b62)

![image](https://github.com/allylikesu/mpd-scripts/assets/100547506/323ebb4a-ad77-43cd-bf65-2791117c60f0)

Dunst notification daemon, Catppuccin color scheme.
(Note: Nerd Font icons are used for play/pause icons in these screenshots. The script in this repo have play/pause emojis instead.)

## mpd-volume
Takes one argument, formatted as [+-]<num>. For example `mpd-volume +5` will increase volume by 5%, and `mpd-volume -2` will decrease volume by 2%. Script will exit with an error code if this argument is blank. Will send a notification with a bar showing the new volume.

![image](https://github.com/allylikesu/mpd-scripts/assets/100547506/3e512d71-dc9a-4f1c-9101-f555774ca4bc)

Dunst notification daemon, Catppuccin color scheme.

## songinfo
From the [ArchWiki article on ncmpcpp](https://wiki.archlinux.org/title/Ncmpcpp#With_album_art). Shows a desktop notification with the current playing track, with album art. Edit `musicdir` and `previewdir` to match your setup. Make sure `previewdir` exists, or else album are will not work.
