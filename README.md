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

Displays a list of all files in the current directory (including all subfolders). You can then type the name of a file, press Enter and it opens according to your rifle configuration. A video demostration of this script can be found [here](https://user-images.githubusercontent.com/41787099/119257229-9bfd8780-bbc4-11eb-8da4-6089de47cf38.mp4).

Uses [fzf](https://github.com/junegunn/fzf) and rifle (provided by the [ranger](https://github.com/ranger/ranger) file manager).

## mnt & umnt

**mnt** mounts devices (or files containing a filesystem) by first creating a folder in /mnt/ and mounting the device/file to it.

**umnt** unmounts devices/files by unmounting it from the folder previously created in /mnt/ and then deletes the folder.

Example:
```
$ mnt /dev/sda1
Mounting "/dev/sda1" to "/mnt/sda1".
$ umnt /dev/sda1 **OR** umnt /mnt/sda1 **OR** umnt sda1
Unmounting "/mnt/sda1".
```

A video demostration of these scripts can be found [here](https://user-images.githubusercontent.com/41787099/119257233-9dc74b00-bbc4-11eb-9ecd-0446925ab41f.mp4).

*These scripts use sudo internally, so make sure that you have sudo access!*

## midiplay & midiserver

**midiplay** plays a MIDI file.

**midiserver** starts a MIDI server so that other applications (MidiEditor, DOSBox etc.) can use MIDI.

A video demonstation of these scripts can be found [here](https://raw.githubusercontent.com/prochazkaml/useful-scripts/master/vids/midi.mkv). **TBD**

Uses [fluidsynth](https://github.com/FluidSynth/fluidsynth) and the [Fluid R3 Soundfont](https://member.keymusician.com/Member/FluidR3_GM/index.html).
