# TF5NN site

The source for a personal site: a front page that links to the apps, and a list of posts with tags and two dates each. It comes in two languages, English and Icelandic, with a switch in the top bar.

It is built with [Hugo](https://gohugo.io/), a program that turns the text files in this folder into web pages. You never have to run Hugo yourself. Once the site is live, GitHub runs it for you every time something changes.

## What is in this folder

| Folder or file | What it is |
|---|---|
| `content/en/` | Everything written in English. |
| `content/is/` | Everything written in Icelandic. |
| `content/en/posts/`, `content/is/posts/` | Your posts. One text file per post. |
| `content/en/apps/` | The pages about each app: overview, instructions, how it came to be. |
| `content/en/about.md`, `content/is/about.md` | The About page in each language. |
| `content/en/_index.md`, `content/is/_index.md` | The headline and introduction on the front page. |
| `static/media/` | Your photos, shared by both languages. |
| `i18n/en.toml`, `i18n/is.toml` | The small fixed texts: button labels, "Posted", "Written up 4 years later", and the Icelandic names of the tags. |
| `hugo.toml` | Site settings: name, tagline and menu links for each language. |
| `.pages.yml` | Settings for the web editor (see below), including the list of tags. |
| `layouts/` and `assets/css/site.css` | The machine: how pages are put together and how they look. You rarely touch these. |
| `.github/workflows/pages.yml` | Tells GitHub how to build and publish the site. |

## Two languages

English is at the main address and Icelandic is under `/is/`. The **EN / IS** switch in the top bar goes to the same page in the other language.

**You only ever have to write a post once, in either language.** Put it in the folder of the language you wrote it in:

- written in English: `content/en/posts/`
- written in Icelandic: `content/is/posts/`

The site then shows it on both sides. On the side where it is missing, the post appears in its original language with a label such as "Icelandic only" or "Aðeins á ensku".

### Adding a translation

A translation is a second file **with exactly the same file name**, in the other language's folder:

```
content/is/posts/2026-11-12-efhw-tuner.md     the original, in Icelandic
content/en/posts/2026-11-12-efhw-tuner.md     the English translation
```

The same file name is what tells the site the two belong together. From then on each side shows its own version, the label disappears, and the switch flips between them.

To say that a post is a translation, add these lines to the translated file:

```
translated_from: is
translated_by: ai
```

`translated_from` is `is` or `en`, the language of the original. `translated_by: ai` is optional. With both lines the post shows "Translated from Icelandic with AI, checked by me." and a link to the original. Without the second line it says just "Translated from Icelandic."

### Having Claude translate a post

1. Post in either language as usual.
2. Tell Claude: "I just posted on my site, please translate it."
3. Claude reads the post, writes the other version and shows it to you.
4. When you approve it, Claude adds the file with the same name in the other folder.

Step 4 needs Claude to have permission to write to this repository on GitHub. Without it, Claude hands you the file and you upload it into the other language's `posts` folder yourself.

### Pages that are not posts

The front page, About page and section titles exist in both languages. The app pages are written in English only, so the Icelandic side shows them in English with a note. To translate one, add a file with the same name under `content/is/apps/`, in the same way as a post.

Links inside your text work in both languages: write `[my apps](/apps/)` and each side points to its own version.

## Writing a post

A post starts with a short block of facts between two `---` lines, followed by the text:

```
---
title: "EFHW tuner in a printed box"
date: 2026-11-12
worked_on: "Spring 2022"
tags: ["HAM radio", "3D printing"]
cover: /media/tuner.jpg
---

The text of the post goes here. It can be one sentence or ten pages.
```

| Line | Meaning | Needed? |
|---|---|---|
| `title` | The headline. | Yes |
| `date` | The day the post goes on the site, as year-month-day. | Yes |
| `worked_on` | When it actually happened, in your own words. | No |
| `tags` | One or more tags. | No |
| `cover` | The main photo, shown at the top and as the small picture in lists. | No |
| `cover_alt` | One sentence describing the main photo for people who cannot see it. | No |
| `summary` | Text shown under the title in lists. Without it, the first paragraph is used. | No |
| `draft: true` | Keeps the post off the site until you remove the line. | No |
| `translated_from`, `translated_by` | Only on a translation. See above. | No |

### The two dates

`date` is always the real day you posted. `worked_on` is free text, so it can be as exact or as vague as your memory, in either language:

```
worked_on: "2022"
worked_on: "Summer 2022"
worked_on: "mars–júní 2022"
worked_on: "2019–2021"
worked_on: "14 August 2022"
```

The site finds the year in that text. If it is earlier than the year you posted, the post gets a note such as "Written up 4 years later". The Timeline page sorts posts by that year (for a range, the last year). Leave `worked_on` out when you post about something you just did.

### Three ways to add a post

**1. Pages CMS, a web editor with a form (easiest).** Go to [app.pagescms.org](https://app.pagescms.org), sign in with GitHub, install its GitHub app on this repository, and open the repository. There is one list for English posts and one for Icelandic posts. Each gives you a form with a title box, date picker, tag list, photo upload and a text editor. Saving puts the post in this repository.

**2. Directly on GitHub.** Open `content/en/posts/` or `content/is/posts/`, choose **Add file → Create new file**, name it something like `2026-11-12-efhw-tuner.md`, paste the block above, write, and choose **Commit changes**. Upload photos the same way into `static/media/`.

**3. On your own computer.** Edit the files in any text editor and send them to GitHub with GitHub Desktop.

Use only plain letters, numbers and dashes in file names, with no Icelandic letters or spaces. The file name becomes the web address of the post.

### Writing the text

The text uses Markdown, which is plain text with a few signs:

```
## A heading

A paragraph. **Bold**, *italic*, and [a link](https://example.com).

- a list item
- another one

![What the photo shows](/media/photo.jpg "An optional caption")
```

The example posts show all of this. Delete them when you have your own.

## Photos

Put photos in `static/media/` and refer to them as `/media/filename.jpg`. The site makes small, fast versions by itself, so a photo straight from a phone is fine to use.

The originals do stay in the repository, and GitHub recommends keeping a repository under about 1 GB. If you post a lot of photos, shrink them to around 2000 pixels wide before uploading.

Use simple file names: lowercase letters, numbers and dashes, no spaces.

## Tags

A tag exists as soon as one post uses it. Write tags the same way in both languages, for example `Metalworking` in an Icelandic post too. That is how the site knows an English post and an Icelandic post share a tag.

What the Icelandic side shows instead is decided in `i18n/is.toml`, in lines like:

```
tag_metalworking = "Málmsmíði"
```

The part after `tag_` is the tag in lowercase with dashes for spaces. A tag without such a line is shown as written, which suits names like SOTA and POTA.

The web editor offers a fixed list so the spelling stays the same. To add a tag to that list, open `.pages.yml`, find `values:` under `tags` (it appears twice, once per language), and add a line in both.

## Adding another app

Copy one of the folders in `content/en/apps/`, rename it, and change the text and the two links at the top of its `_index.md`. It shows up on the front page and the Apps page by itself, in both languages.

## Keeping it private, and going live later

A free GitHub account can only publish a site from a public repository. So:

**Private (now).** Create a repository named `TF5NN.github.io`, set it to **Private**, and upload this folder. Nothing is published. The publishing step is written to do nothing while the repository is private.

**Live (when you are ready).**

1. Repository **Settings → General → Danger Zone → Change visibility → Public**.
2. **Settings → Pages → Source: GitHub Actions**.
3. **Actions** tab → **Build and publish** → **Run workflow**.

A minute or two later the site is at `https://tf5nn.github.io/`. From then on, every change publishes itself.

The repository name matters. `TF5NN.github.io` is the one name that puts the site at the top address, with the apps already sitting below it at `/sat-track/` and `/HF-Antenna-Impedance-Visualizer/`.

## Your own domain, later

1. Buy the domain from any registrar.
2. In **Settings → Pages → Custom domain**, type the domain and save.
3. At the registrar, add the DNS records GitHub asks for. The steps are in GitHub's guide: [Managing a custom domain for your GitHub Pages site](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).
4. Back in **Settings → Pages**, tick **Enforce HTTPS** once it becomes available.

Nothing in this folder needs to change. The apps move to the new domain too, at the same paths. Northbound remembers your station per address, so you enter your location once more after the move.

## Seeing the site on your own computer (optional)

1. Install Hugo, the "extended" edition: [gohugo.io/installation](https://gohugo.io/installation/). The site was made with version 0.169.0, and the way the two languages share posts needs a recent version.
2. Open a terminal in this folder and run `hugo server`.
3. Open `http://localhost:1313` in a browser. The page updates as you save files.

## Changing the look

Colours and fonts are at the top of `assets/css/site.css`. They are the same values the two apps use, so the site and the apps look like one place. If you change them here, change them in the apps too.

## Your email address

The address is set once, in `hugo.toml` (`email_user` and `email_domain`). To show it on any page, write a link to `#email`:

```
[email](#email)
```

In the web editor's normal view, select a word and use the link button with `#email` as the address. Readers see a normal clickable address. The page itself only holds a scrambled copy, plus "gunnar.bjarki (at) gmail.com" for anyone without scripts, which keeps it away from simple spam bots. `{{</* email */>}}` does the same thing if you prefer typing it in Source view.

## Visit counting

The site counts visits anonymously with GoatCounter, in the same account as the apps (tf5nn.goatcounter.com). It uses no cookies and records no personal details. To turn it off, empty the `goatcounter` line in `hugo.toml`.
