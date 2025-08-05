# Keybindings for VSCode on MacOS.

## Motivation

When using Vim Keybindings in VSCode, there are still times one might need to reach for the arrow keys. E.g. when selecting a file, or a code action.

These keybindings use native vim navigation `(j, k) + cmd` for navigating these sections.

### Features

- Navigate all drop down menus with `cmd+j`/`cmd+k`
- Navigate left/right with `cmd+h`/`cmd+l`
- Navigate inner buffers (editors tabs, terminals) with `cmd+n`/`cmd+m`

- Copy/paste/delete files in the file explorer with `y`/`p`/`d`
- Extract current editor/terminal into a new group with `cmd+shift+h`/`cmd+shift+l`
- Close current editor/terminal with `cmd+w`
- Show/hide the sidebars with `cmd+e` and `cmd+;`
- Navigate search results with `j`/`k`

### TODO

- Navigate up/down with `cmd+j`/`cmd+k` (currently, terminal is toggled with `cmd+j` and `cmd+k` is used for inline terminal chat in Cursor)
- While `cmd+j` moves downwards from the search box to the results, it does not work if search details are toggled.

## Usage

These keybindings work for both VSCode and Cursor.

### VSCode

```sh
cp keybindings.json ~/Library/Application\ Support/Code/User/keybindings.json
```

### Cursor

For these keybindings to work, make sure to set `workbench.activityBar.orientation` to `vertical` in your settings.json file.

Then, copy the keybindings:

```sh
cp keybindings.json ~/Library/Application\ Support/Cursor/User/keybindings.json
```

## Contributing

If you made changes to the keybindings and you are using VSCode, you can update this repository with:

```sh
cp ~/Library/Application\ Support/Code/User/keybindings.json keybindings.json
```

for Cursor, you can update the file with:

```sh
cp ~/Library/Application\ Support/Cursor/User/keybindings.json keybindings.json
```