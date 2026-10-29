# NeuroKind Games website

A single page: `index.html`, plus the pictures in `img/`. There's nothing to build or install.

## 1. Add your links
Open `index.html` in Notepad and scroll to the bottom. There's a list called `LINKS`: paste each game's address between its quotes, for example:

    unrest: 'https://yourname.itch.io/unrest',

- A game with no link yet shows "Coming soon".
- The books and YouTube buttons stay hidden until you add their links.

## 2. Put it on GitHub Pages (free)
The site lives at **https://c0gn8.github.io**. For GitHub to serve it at that address (with nothing after the `.io`), the repository must be named exactly `c0gn8.github.io`.
1. Sign in at github.com as **c0gn8** and create a new **public** repository called `c0gn8.github.io`.
2. Click **uploading an existing file** and drag in everything from this folder: `index.html`, `privacy.html`, `README.md` and the `img` folder. Then click **Commit changes**.
3. Go to **Settings → Pages**. Under "Build and deployment", choose **Deploy from a branch**, pick **main** and **/ (root)**, then click **Save**.
4. After a minute or two the site is live at `https://c0gn8.github.io`.

If you already uploaded the site to a repository with a different name, either rename that repository to `c0gn8.github.io` (Settings → General → Repository name), or the site's address will be `https://c0gn8.github.io/<repository name>/` and the links below need that added.

## Changing things later
- **Words:** edit them in `index.html`.
- **Pictures:** replace the matching file in `img/` with one of the same name. Wide pictures (16:9) suit the game cards best.
- **Adding a game:** copy one of the `<article class="game">` blocks, change the words and picture, and give it a new name in `LINKS`.

## Privacy policy
`privacy.html` is the studio's privacy policy, linked from the footer of the home page. Once the site is live, its address is `https://c0gn8.github.io/privacy.html`: use that in the Google Play Console (App content → Privacy policy) and on your itch.io and Roblox pages. Update the "Last updated" date whenever you change it.
