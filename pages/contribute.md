You have some free time and want to contrbute to this wiki?
Or you simply found a mistake somewhere and want to correct it?

Every page on this wiki is **open-source**, which means everyone can change, add or update it!

## 1: Understand GitHub

The main repository of the wiki is hosted on GitHub, powerfull website for open-source projects.

You'll need to create an account (if you don't own one already), then **fork** the [**DiSkyDocs**](https://github.com/DiSkyOrg/DiSkyDocs) repository.

Wait a few minutes while your new repository is being setup, and there you go! Your personal edition of this repository will **not** affect the original repository.

## 2: Files organisation

You **must not** change how files & folders are organised. Here's a quick recap of main contents:

* `pages/` - Where every page's content is stored, written in **MarkDown**
* `static/` - Where every static-content, such as video, image etc., is stored.
* `data.json` - Where every page's data such as name, title and file is stored, written in **JSON**
* `emojis.json` - Where all emojis are stored, to be replaced in markdown content, written in **JSON**
* `logo.png` - The main DiSky's logo, currently unused.

## 3: Contributing your changes

When you have edited, added or removed the desired files, you can open a **pull request**, sort of a GitHub issue that sums up everything you've changed, in the [**DiSkyDocs**](https://github.com/DiSkyOrg/DiSkyDocs) repository.

Me, Sky, and other validated contributors will review your changes, requesting changes if needed.

Once half of the validated contributors approve of your changes, and there's nothing left to review, we'll move your pull request, and all of your changes with it.

> :warning: **Sky** has to be online in order to **upload** the new files on the **wiki's server**! It could take a few days before the page refreshes!

## Example: Editing an existing page

1. Search the page's content file in `pages/` folder. The file name must be the **page's ID** (what's written in the URL parameter).
2. Open the file (through GitHub editor, or download it to upload it later).
3. Make your modifications and save your files.

Go into part `3)` in order to contribute your changes.

## Example: Creating a new page

1. Edit the `data.json` file, create a new section similar to the other already present, write your page name, title and it's id.
2. Create a new file called `<page id you specified above>.md` **in** the `pages/` folder.
3. Edit the page's file you've created above with your content, and save it.

> :warning: Don't forget to also save the `data.json` file!

Go into part `3)` in order to contribute your changes.
