# Amanda Panda Helps Ya' Standa — Website

This folder is a complete, ready-to-deploy website. It's plain HTML/CSS/JS —
no build step, no npm install, nothing to compile. That makes Netlify's
simplest deploy method a perfect fit.

## What's in here

```
index.html      the whole site (one page, all sections)
thanks.html     the page visitors land on after submitting the contact form
favicon.*, apple-touch-icon.png, icon-*.png, site.webmanifest   browser tab and home-screen icons
images/         all photos, logos, and badges used on the site
audio/phrases/  the 7 individual real recorded phrase clips (phrase1.mp3 ... phrase7.mp3)
```

## Deploy to Netlify (drag-and-drop, ~2 minutes)

**On a Chromebook, or anywhere folder drag-and-drop is finicky: just drag in
the `.zip` file itself, unopened.** Netlify accepts a zip directly and
unzips it for you — you don't need to extract it first. This zip is
packaged with `index.html` at the top level (not inside a subfolder), so it
publishes correctly at your site's root either way.

1. Go to https://app.netlify.com and log in (or create a free account).
2. On your dashboard, look for the box that says **"Drag and drop your site
   output folder here."**
3. Drag the downloaded `.zip` file straight into that box (no need to
   unzip it first — Chromebook, Mac, or Windows all work this way).
4. Netlify uploads and unzips it, then gives you a live URL in a few
   seconds, something like `random-name-123.netlify.app`. The site is now
   live at that root URL — not inside any subfolder.

That's it — no code, no terminal, no extracting.

**Redeploying after a future update:** every time I send you a new zip,
repeat the same step — drag the new zip into the same site's deploy box
(or the "Deploys" tab → drag in the new zip there). Each drop creates a
fresh deploy that fully replaces the last one.

## Connecting amandapandahelpsyastanda.com

1. In Netlify, open your new site, then go to **Site configuration → Domain
   management → Add a custom domain**.
2. Enter `amandapandahelpsyastanda.com` and follow the prompts.
3. Netlify will show you either:
   - **Nameservers to switch to** (easiest — Netlify manages all DNS for
     you), or
   - **A few DNS records to add** at whichever registrar you bought the
     domain from (GoDaddy, Namecheap, etc.), if you'd rather keep DNS there.
4. DNS changes can take anywhere from a few minutes to a few hours to fully
   go live. Netlify issues a free HTTPS certificate automatically once it
   sees the domain pointed at it — no extra step needed.

## The contact form

The "Licensing, press, or just want updates?" form at the bottom of the
page is wired up for **Netlify Forms**, which means:

- No backend, no email service to configure.
- Once the site is deployed on Netlify (drag-and-drop is enough — this
  works without connecting to GitHub), Netlify automatically detects the
  form and starts collecting submissions.
- You'll find every submission under your site's **Forms** tab in the
  Netlify dashboard, and you can turn on **email notifications** there so
  submissions land in your inbox too (Site configuration → Forms →
  Notifications).
- There's a hidden "honeypot" field built in to filter out spam bots — you
  don't need to do anything for that to work.

## Making updates later

Since this is one HTML file, small changes (a new phrase, an updated status
chip, a different email address) can be made by opening `index.html` in any
text editor, editing the text between the tags, saving, and dragging the
folder into Netlify again — it'll create a new deploy in a few seconds. If
you'd rather not touch code by hand, send the change to Claude along with
this project and ask for an updated `index.html`.

## If you want it on GitHub instead (optional)

Drag-and-drop is the simplest path and is perfectly fine long-term. If you
later want automatic redeploys whenever a file changes (e.g. working with a
developer), you can instead push this folder to a GitHub repository and
connect that repository in Netlify under **Add new site → Import an
existing project**. Not necessary to get started.

## Notes on the content

- The "Press the Button" paw icon now plays the **real recorded audio** for
  each phrase — every press plays the matching line from your original
  recording (`amanda_panda_voice_lines.wav`), split into 7 individual clips
  under `audio/phrases/`. The recording says the script twice; the clips
  come from the first pass. Each phrase was identified by ear and cut at the
  pauses around it, with a little padding so no word is clipped.
- The contact form's "I'm reaching out as a…" options and the status chips
  ("Working Prototype," "Tested by 6+ Families," etc.) reflect the current
  state of the project — update them if that changes.
- The "Shared With Friends & Family" stories in the Our Story section are
  based on what you've told me about specific families who tried
  prototypes. If any names, details, or outcomes need correcting, just say
  so and I'll update the copy.
