# `colorscheme.sh` Usage


> **Note:** The following example commands assume your current directory is the root of the `termux` repo.

---

## Installing the `colorscheme` script

1. Symlink the script into your path
2. Make the .sh file executable

### Symlink the .sh file

```
# make the .sh executable
chmod +x bin/colorscheme.sh

# symlink it to your bin folder or any folder in yohr path
ln -s bin/colorscheme.sh ~/bin/colorscheme
```

## `colorscheme` Usage

Running: 

```
colorscheme
```

Will display a list of color schemes with previews. You can cycle through the list and press `enter` on one to set it.

Sucsessfully setting a scheme executes the following:

```
clear && rm colors.properties && ln -s $scheme colors.properties && termux-reload-settings && neofetch && lll
```

Thus providing an immediate preview

### Options

The `colorscheme` script has the following options:

- `-s | --set` - Same as running `colorscheme` with no options. Brings up interactive menu
- `-s | --set <name or path>` - Adding a name or path after `--set`. Sets a new color scheme by name or path. Name alone is sufficient, but a path can be privided as well
- `-h | --help` - Displays help page
- `-l | --list` - Lists color schemes with previews. Same as `--set` with no path
- `-l | --list <type:premade|custom|favorites>` - Lists color schemes of that type
- `--<premade|custom|favorites>` - displays list of schemes of that type. Options are `--premade`, `--custom` , `--favorites`. Same as the `--list` option with a type provided,