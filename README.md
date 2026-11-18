# Leapfall website

These are standalone static files for the existing leapfall.com GitHub Pages site.
There is no build step, JavaScript, framework, analytics or game/server dependency.

## Upload to GitHub Pages

1. Download this complete `website` folder from the project. Keep `assets` and all the files inside it together.
2. Open your existing website repository on GitHub. Before replacing files, keep a copy of the current site.
3. Check the repository's **Settings → Pages** to see its current publishing branch and folder. Keep that existing setup.
4. In that publishing folder, choose **Add file → Upload files**. Upload the **contents** of `website`, not the enclosing `website` folder: the four HTML files, `README.md`, and the complete `assets` folder. If your site publishes from `/docs`, these files go inside `docs` instead.
5. Keep any existing `CNAME` file and your leapfall.com custom-domain/DNS settings. This export deliberately doesn't replace them. Don't delete unrelated repository configuration.
6. Commit the upload. GitHub Pages will update the website after it finishes processing the commit. This is your manual publishing step; nothing has been uploaded from Replit.
7. Check Home, Privacy, Terms and Delete my data on leapfall.com, including on a phone. Each page should load its fonts and images, and the Contact links should open an email to hello@leapfall.com.

The game does **not** need a native sync or server republish for these website files.
The site uses relative asset/navigation paths, so it also works at a GitHub Pages repository subpath. Canonical and share-preview URLs intentionally point to the final leapfall.com domain.

## Add the store links later

Open `index.html` and find the two comments:

- `Replace with real App Store link when live`
- `Replace with real Google Play link when live`

Each placeholder is currently a disabled button labelled **Link coming soon**. To activate one, replace that whole button with a link using the same `store` class. For example:

```html
<a class="store" href="PASTE_THE_REAL_STORE_URL_HERE">
  <b>App Store</b><small>Download on the App Store</small>
</a>
```

Use the equivalent Google Play wording for the other link. Do not leave the example URL or a `disabled` attribute in a live link.

## Legal wording

The legal body text and dates are the wording supplied by the owner. The Privacy page's pending in-app purchases section remains in the file but hidden, as supplied.
The deletion page adds a separate **Settings → Delete my data** instruction.
Existing legal claims have not been fact-checked or rewritten. In particular, statements about server-stored progress remain exactly as supplied; this styling work is not a legal or data-storage audit.

## Artwork

- `feature-graphic.png`: existing store feature graphic, showing the actual frog, waterfall and Aicon wordmark. Also used as the social share preview.
- `home-frog.png`: the existing Home/intro frog render, with only transparent outer margins trimmed. No AI imagery.
- `gameplay-1.png`, `gameplay-2.png`, `gameplay-3.png`: genuine captures of the game running locally in Misty Rainforest, before and during jumps. Captured in an isolated browser with API requests blocked; no scores or player data were sent. These are not mockups or promises of different biomes.
- Fonts and icon: copies of the game's existing files. The owner remains responsible for applicable font redistribution/web-use rights.

## Complete file list

```text
index.html
privacy.html
terms.html
delete-account.html
README.md
assets/site.css
assets/aicon-regular.ttf
assets/aicon-bold.otf
assets/aicon-extra-bold.otf
assets/feature-graphic.png
assets/home-frog.png
assets/icon-512.png
assets/gameplay-1.png
assets/gameplay-2.png
assets/gameplay-3.png
```
