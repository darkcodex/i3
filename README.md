# i3
 Tiling window manager
 
 #Install i3 package group (includes window manager, screenlocker and a status bar).  
 
   sudo pacman -S i3

#Install dmenu:

   sudo pacman -S dmenu

#Install ranger for file manager:
 
   sudo pacman -S ranger

#Install vim text editor:

   sudo pacman -S vim

#Tell you how to make it your default editor, thought. It is pretty easy. 
Just go to ~/.bashrc:

   export VISUAL=vim
   export EDITOR=vim

#Install feh for background:

   sudo pacman -S feh

#Install zathura the pdf reader:

   sudo pacman -S zathura

#Install cmus music player:
   sudo pacman -S cms
and vlc:
   sudo pacman -S vlc

#Basic shortcuts i3:

   modkey + return to start a terminal.
   modkey + shift + q to close current window.
   modkey + f switches the active window to fullscreen view.
   modkey + d for dmenu.
   modkey + shift + e to kill i3 session.

#Mutimedia key:
Install playerctl from the AUR 

   yaourt -S playerctl

Then you can add this lines to your ~/.i3/config.

# Multimedia Keys
# increase volume
bindsym XF86AudioRaiseVolume exec amixer -q set Master 5%+ unmute
# decrease volume
bindsym XF86AudioLowerVolume exec amixer -q set Master 5%- unmute
# mute volume
bindsym XF86AudioMute exec amixer -q set Master mute
# pause / play / next / previous
bindsym XF86AudioPlay exec playerctl play-pause
bindsym XF86AudioNext exec playerctl next
bindsym XF86AudioPrev exec playerctl previous

#Configuring GTK without a GUI

   sudo pacman -S lxappearance
