# Using this Repo


### Installing this repo into your `.termux` Folder as a submodule

```
git submodule add --name colors -b termux https://github.com/8rents/colors
```

The `termux` branch of this repository is designed to be imported into the `Termux` repository as a submodule.

The relative symlink already exists, linking the `premade` directory to `.submodules/termux-styling/app/src/main/assets/colors`. Make sure when you `clone` the `termux` repository to use `--recurse-submodules` flag.

### Folders in this repo

```
$HOME/dotfiles/termux/colors
```

This directory holds all color informtion.

- `premade` holds themes that are included in the termux styling  app.
- `custom` holds themes I've made or modified
- `screenshots` holds screenshots for quick reference
- `favorites` holds symlinks from the `custom` and `premade` folders to keep a curated collection. 
