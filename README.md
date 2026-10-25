# NeuroKind Games website

A single page: `index.html`, plus the pictures in `img/`. There's nothing to build or install.

## 1. Add your links
Open `index.html` in Notepad and scroll to the bottom. There's a list called `LINKS`: paste each game's address between its quotes, for example:

    unrest: 'https://yourname.itch.io/unrest',

- A game with no link yet shows "Coming soon".
- The books and YouTube buttons stay hidden until you add their links.

## 2. Put it on GitHub Pages (free)
1. Sign in at github.com and create a new **public** repository, for example `neurokind-site`.
2. Click **uploading an existing file** and drag in everything from this folder: `index.html`, `CNAME`, `README.md` and the `img` folder. Then click **Commit changes**.
3. Go to **Settings → Pages**. Under "Build and deployment", choose **Deploy from a branch**, pick **main** and **/ (root)**, then click **Save**.
4. After a minute or two the site is live at `https://<your-github-name>.github.io/neurokind-site/`.

## 3. Point olidnejad.com at it
In your domain's DNS settings (Squarespace → Domains → olidnejad.com → DNS):
1. Delete the existing Squarespace records for `@` and `www`.
2. Add four **A** records for host `@`, one for each of these addresses:
   - 185.199.108.153
   - 185.199.109.153
   - 185.199.110.153
   - 185.199.111.153
3. Add a **CNAME** record for host `www` pointing to `<your-github-name>.github.io`.
4. Back on GitHub, go to **Settings → Pages**. Under "Custom domain" type `olidnejad.com` and click **Save**. Once the check passes (it can take up to a day), tick **Enforce HTTPS**.

**Before you cancel Squarespace,** make sure the domain stays registered. If Squarespace is your domain registrar, keep the domain renewing there (it's billed separately from the website plan), or transfer it to another registrar first.

## Changing things later
- **Words:** edit them in `index.html`.
- **Pictures:** replace the matching file in `img/` with one of the same name. Wide pictures (16:9) suit the game cards best.
- **Adding a game:** copy one of the `<article class="game">` blocks, change the words and picture, and give it a new name in `LINKS`.
