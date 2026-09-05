# How to update your website

You never need to touch code. You edit plain text files in the **`content`** folder,
then ask Claude to rebuild the site.

---

## The three steps

### 1. Edit your text

Open the **`content`** folder. Inside are seven files, one for each page of your site:

| File | Is the page |
|---|---|
| `1-homepage.md` | Your front page |
| `2-field-photos.md` | Photos from the Field |
| `3-dissertation.md` | Dissertation Research |
| `4-teaching.md` | Teaching |
| `5-publications.md` | Publications |
| `6-before-the-phd.md` | Pre-PhD |

Open any of them in TextEdit (or any editor) and change the words. Each file
explains itself at the top.

**The one rule:** keep the labels — the words ending in a colon, like `Story:` or
`Where:` — exactly as they are. Change only the text *after* them.

If you break something, it is fine. Claude will tell you what looks wrong instead
of building a broken page.

### 2. Ask Claude to rebuild

Open this folder in Claude Code and type:

```
/update-website
```

That is the whole command. Claude reads your files, rebuilds every page, checks
that nothing is broken, and tells you in plain language what changed.

If something in your text was unclear, Claude will ask you about it rather than guess.

### 3. Publish

Claude will show you exactly what to copy and paste to publish, and will offer to
do it for you. Nothing goes live on the internet until you say yes.

---

## Adding a new photo

1. Put the photo file into the **`field`** folder.
2. Open `content/2-field-photos.md`.
3. Copy one of the existing photo blocks, paste it at the bottom, and change the
   file name.
4. Run `/update-website`.

Your photos are never cropped — whatever shape they are, they are shown whole.
If you forget step 3, Claude will notice the new photo and ask you what to say
about it.

## Adding a description to a photo

Every photo in `content/2-field-photos.md` has two blank lines waiting:

```
Label:
Description:
```

Fill in either one and a caption panel appears under that photo. Leave both
blank and the photo stays plain. You can caption some photos and not others.

- **Label** — a few words: a place, a date, a kind of work. Shown small and in
  capitals above the description.
- **Description** — a sentence or two about the photograph.

---

## Things worth knowing

**Photo file names are fussy about capital letters.** `Photo.JPG` and
`photo.jpg` are different names as far as the website is concerned, even though
your Mac treats them as the same. This broke two images on the live site once
already. Every photo is now named in lowercase — keep new ones lowercase too,
and Claude will check before you publish.

**Changes take a minute or two to appear** on the live site after you publish.
If you do not see them, wait a moment and refresh.

**You cannot break the design.** The layout, colours, and fonts live in files you
never open. The worst that happens is a typo, and you fix it by editing the text
and running `/update-website` again.

---

## If you get stuck

Just describe the problem to Claude in your own words — for example:

> The third photo on my field page is showing the wrong caption

> I want to add a publication from 2026

> Can the homepage say Assistant Professor instead of Visiting Assistant Professor

You do not need to know the technical terms. Describe what you want and Claude
will find the right file and make the change.
