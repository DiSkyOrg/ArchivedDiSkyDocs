You have some free time and want to contrbute to this wiki?
Or you simply found a mistake somewhere?

Every pages of this wiki **open-source**, means everyone can change, add or update other's works!

## 1: Understand GitHub

The main repository of the wiki is hosted on GitHub, powerfull website for open-source projects.

You'll need to create an account (if you don't own one already), then **fork** the [**DiSkyDocs**](https://github.com/DiSkyOrg/DiSkyDocs) repository.

Wait some minutes until your new repository is being setup, and here you go! Your personal edition on this repository will **not** affect the original repository.

## 2: Files organisation

You **must not** change how are organised files & folders. Here's a quick recap of main contents:

* `pages/` - Where every page's content are stored, written in **MarkDown**
* `static/` - Where every static-content, such as video, image and other, are stored.
* `data.json` - Where every page's data such as name, title and file are stored, written in **JSON**
* `emojis.json` - Where every emojis are stored, to be replaced in markdown content, written in **JSON**
* `logo.png` - The main DiSky's logo, currently unused.

## 3: Contributing your changes

When you have edited, added or removed the desired files, you can open a **pull request**, sort of GitHub issue that's sum up everything you changed, in the [**DiSkyDocs**](https://github.com/DiSkyOrg/DiSkyDocs) repository.

Me, Sky, and other validated contributors will review your changes, reuesting changes if needed.

Once half of the validated contributors approved your changed, and there's nothing left to review, we'll move your pull request, and therefore all of your changes.

> :warning: **Sky** need to be online in order to **upload** the new files on the **wiki's server**! It could take some days before refreshing!

## Example: Editing an existing page

1. Search the page's content file in `pages/` folder. The file name must be the **page's ID** (what's written in the URL parameter).
2. Open the file (through GitHub editor, or download it to upload it later).
3. Make your modification and save your files.

Go into part `3)` in order to contribute your changes.

## Example: Creating a new page

1. Edit the `data.json` files, create a new section similar to other alreay present, and write your page name, title and id.
2. Create a new file called `<page id you specified above>.md` **into** `pages/` folder.
3. Edit the page's content file you created above with your needs, and save it.

> :warning: Don't forget to also save the `data.json` file!

Go into part `3)` in order to contribute your changes.