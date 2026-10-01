# Yiming Ling — personal website

Static site (no build step required to serve). Structure:

```
index.html          English page
index_zh.html       Chinese page
assets/css/style.css
assets/js/main.js
assets/images/avatar.svg   (initials avatar / favicon — replace with a photo if you like)
assets/cv/YimingLing_CV.pdf
```

## Publish on GitHub Pages (account: YimingLG)
1. On GitHub, create a new **public** repository named exactly `YimingLG.github.io`.
2. Upload the contents of this folder to the repository root (`index.html` must be at the top level):
   *Add file → Upload files*, drag everything in, commit. Or from a terminal:
   ```
   git clone https://github.com/YimingLG/YimingLG.github.io.git
   cd YimingLG.github.io   # copy the site files here
   git add . && git commit -m "Personal website" && git push
   ```
3. In *Settings → Pages*, set *Source* to "Deploy from a branch", branch `main`, folder `/ (root)`.
   The site goes live at **https://yiminglg.github.io/** within a minute or two.
4. Optional: put that URL in the *Website* field of your GitHub profile.

## Common edits
- **Photo:** put `photo.jpg` in `assets/images/` and change `assets/images/avatar.svg` to
  `assets/images/photo.jpg` in the `<img class="brand-avatar">` tag of both HTML files.
- **Profiles (GitHub / Google Scholar / ORCID):** uncomment and fill the links in the *Contact* section.
- **New CV:** replace `assets/cv/YimingLing_CV.pdf` (keep the filename, or update the links).
- **Colours / fonts:** the variables at the top of `assets/css/style.css` (`--primary`, fonts).
