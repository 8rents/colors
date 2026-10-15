# termux colors submodules

> *Submodules to assist in coloring termux beautifully*

---

## termux styling colors symlink

*from root of colors repo*

> - look up init cmd
> - look up ts gh repo

```
# add styling as submodule
git submodule add --name termux-styling https://github.com/ submodules/termux-styling --depth 1

# initialize it
git submodules init --recurse

# symlimk the colors directory as premade
ln -s submodules/termux-styling/app/src/main/assets/colors premade
```