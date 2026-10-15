# Color Scheme  Documentation

*note that this isw only the `docs`  branch. There are no color schemes or app config files on this branch. This is the `[default]` front facing branch on GitHub and only contains platform and aapplication agnostic information.*

> *Creating color schemes for a variety of different applications, some of the applications are simply the love of color combinations*

---

## Repository Structure

The repository has all development and completed schemes and application configs within the development directory.]

### When developing a scheme...

- I will be working on the `dev` branch ihn the` Development` to develop new schemes
- When a scheme is completed, it will be moved out of the `Development` branvh and in to the `Finished` folder. Within the finished folder there are screenshots to quickly be able to preview themes.

### Using Colors as a  standalone development repo

However when a new scheme is complete I will move it into the application folder. The list of folders in `applications` is the list of apps that are going to support the color scheme.

### Exporting finished color schemes to specific applications

Once the application folder has been filled out, I will create a new branch in the repo from the `blank` branch, named after thr application that the exported color schemes are going to support.

#### Example branches

- `dev`
- `blank`
- `docs`
- `termux` - this branch will only have the termux color scheme

### Importing an application branch into a parent repository

Here when I want to import termux color schemes into termux I will cone this repository with the `-b` flag and only clone the `termux` branch. 	I will also use the `--depth 1`  flag to only get the most recent version of the repo. Really just the most recent version of the specific branch that I need to work with in termux. 

#### To sparse-checkout or not to sparse checkout	

I might also seem like a good idea to do a sparse checkout to only grt the exact files that I'll need. However that won't be necessary.  	Since I created the application branch from the `blank` branch, the only things I'm downloading in the repo are only the exact things that I need to get my ccolor goals accomplished.
 
---

🤍 2024 **[Brenton Holiday](https://allmylinks.com/8rents)** 