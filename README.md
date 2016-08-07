# OSX and Sublime Text like keymap for IntelliJ

A keymap, based on the 'default' Mac OS X 10.5 keymap from IntelliJ, which overrides things back to 'normal' OS X keymaps, like top of file with `cmd + up`, delete everything to the beginning of the line with `cmd + backspace` etc. It also set's the keybindings to be comparible with Sublime Text, with some small exceptions.

## Installation instructions

1. If you have IntelliJ running, close it (completely)

2. Clone this repository
   ```
   git clone git@github.com:peterklijn/osx-and-sublime-like-keymap-in-intellij.git
   ```

3. Symlink the XML file you just cloned to this directory
   ```
   ln -s ~/path/to/git/repo/osx-and-sublime-like-keymap.xml ~/Library/Preferences/IdeaIC2016.2/keymaps/. # Or whatever version of IntelliJ you use
   ```

4. Start IntelliJ, go to the preferences (`cmd + ,`), go to Keymap, select 'OSX and Sublime Text' in the list of available keymaps.

Tested in IntelliJ IDEA Community 2016.2.1

## Removed IntelliJ OSX defaults

- `cmd + down` Jump to source
- `cmd + alt + up` Navigate to previous occurrence
- `cmd + alt + down` Navigate to next occurrence
- `ctrl + G` Add selection to next occurrence
- `cmd + D` Duplicate line or selection
- `cmd + backspace` Delete line
- `cmd + shift + R` Replace in path
- `cmd + alt + F` Extract field (refactor)
- `cmd + P` Parameter info
- `cmd + alt + E` Explain Scala code, Browse console history


## OSX defaults restored

- `cmd + up` Caret to top of file
- `cmd + down` Caret to bottom of file
- `cmd + backspace` Delete to line start

## Sublime defaults added

- `cmd + D` Add selection for next occurrence
- `cmd + shift + D` Duplicate line or selection
- `ctrl + shift + K` Delete line
- `cmd + alt + F` Replace
- `cmd + shift + R` Navigate to Symbol
- `cmd + P` Navigate to file

## Custom stuff

-  `cmd + alt + up` Navigate back
-  `cmd + alt + down` Jump to source

## Todo

- `cmd + alt + F` Extract field (refactor)
