# useful-scripts
Small, yet useful scripts for GNU/Linux systems.

## Installation 

To install the scripts for all users:

```
git clone https://github.com/prochazkaml/useful-scripts
sudo cp -r useful-scripts/scripts/* /usr/bin/
```

Or, if you want to install the scripts just for yourself:

```
git clone https://github.com/prochazkaml/useful-scripts
sudo cp -r useful-scripts/scripts/* ~/.local/bin/
```

## fo

Displays a list of all files in the current directory (including all subfolders). You can then type the name of a file, press Enter and it opens according to your rifle configuration. A demostration of this script can be found [here](https://raw.githubusercontent.com/prochazkaml/useful-scripts/master/vids/fo.mkv). **TBD**

Uses [fzf](https://github.com/junegunn/fzf) and rifle (provided by the [ranger](https://github.com/ranger/ranger) file manager).

## mnt & umnt

**mnt** mounts devices (or files containing a filesystem) by first creating a folder in /mnt/ and mounting the device/file to it.

**umnt** unmounts devices/files by unmounting it from the folder previously created in /mnt/ and then deletes the folder.

A demostration of this script can be found [here](https://raw.githubusercontent.com/prochazkaml/useful-scripts/master/vids/mnt.mkv). **TBD**

*These scripts use sudo internally, so make sure that you have sudo access!*

## midiplay & midiserver

**midiplay** plays a MIDI file.

**midiserver** starts a MIDI server so that other applications (MidiEditor, DOSBox etc.) can use MIDI.

A demostration of this script can be found [here](https://raw.githubusercontent.com/prochazkaml/useful-scripts/master/vids/midi.mkv). **TBD**

Uses [fluidsynth](https://github.com/FluidSynth/fluidsynth) and the [Fluid R3 Soundfont](https://member.keymusician.com/Member/FluidR3_GM/index.html).
