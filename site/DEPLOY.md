# Deploying Min al-Ataba to GitHub Pages

One time setup, run from inside the site folder on your Mac:

```
cd "site"
git init
git add .
git commit -m "Initial scaffold"
```

Create an empty repository on github.com (suggested name: min-al-ataba), then:

```
git remote add origin https://github.com/YOUR_USERNAME/min-al-ataba.git
git branch -M main
git push -u origin main
```

On github.com open the repository, then Settings, then Pages. Under Source choose "Deploy from a branch", branch `main`, folder `/ (root)`. Save. The site goes live within a minute at:

```
https://YOUR_USERNAME.github.io/min-al-ataba/
```

## Publishing an entry during the term

1. Open `index.html`
2. Find the entry section (`id="ataba"`, `id="amanah"`, `id="marifa"`, `id="tarjama"`)
3. Replace each `<p class="forthcoming">Forthcoming.</p>` with your paragraphs in plain `<p>` tags
4. Then:

```
git add index.html
git commit -m "Entry 1"
git push
```

Live in under a minute. The commit history doubles as a record of the journal's development across the term.

## Replacing the calligraphy with your own hand

Photograph or scan your hand lettered word, trace it to SVG (or export PNG with transparent background), drop it into `assets/` with the same filename, and push. Nothing else changes.
