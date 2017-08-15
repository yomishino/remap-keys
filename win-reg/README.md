# A brief description of the .reg files

Here are some .reg files for remapping keys on Windows. They should work for all those popular versions of Windows: Windows XP, 7, 8, 8.1, 10, ...

The mapping is done by adding a value (`"Scancode Map"` under `[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Keyboard Layout]`) in the Windows Registry, which Windows uses to handle the remapping of keys.

# How to use

Download the file you want and then run it by double clicking on it. You will probably be prompted for confirmation. Press yes.

Alternatively, if you are comfortable with directly editing the Regsitry, check the corresponding key and value in the file and mannually edit your Registry. (Not recommended unless you are confident with it.)

## Important notes

Since there is only one value corresponding to the key mapping, the mappings set by the files are non-overlapping. If you run one file and then another, the latter one will overwrite the value. In other words, only the last file you run has the real effect.

And, don't forget to **reboot** your PC to make it work.

## Enough of remapping?

Use [this one](keymap-reset.reg) to reset.
It simply removes the value from the Registry.


# List of files

Currently, there are three files that deal with the **Caps Lock** key:
- [keymap-swap-ctrl-caps.reg](keymap-swap-ctrl-caps.reg):
    For swapping Ctrl and Caps Lock,
- [keymap-caps-to-ctrl.reg](keymap-caps-to-ctrl.reg):
    For mapping Caps Lock to Ctrl,
- [keymap-disable-caps.reg](keymap-disable-caps.reg):
    For completely disabling the Caps Lock.

And lastly, one file to remove (disable) the remapping:
- [keymap-reset.reg](keymap-reset.reg)
