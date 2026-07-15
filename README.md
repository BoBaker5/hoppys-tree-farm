# Hoppy's Christmas Tree Farm — Website

A single-page website for Hoppy's Christmas Tree Farm, a family-run cut-your-own
Christmas tree farm at 108 Ryder Rd, North Stonington, CT 06359.

## What's in here

```
index.html      The entire site — all HTML, CSS, and JavaScript in one file
images/         Optimized web-ready photos and the farm logo
Photos/         Original photos (not part of the published site; ignored by git)
README.md       This file
```

There is no build step, no framework, and nothing to install. **Just open
`index.html` in a browser** — double-click it, or drag it onto a browser window.

## Editing the site

Everything lives in `index.html`:

- **Text/content** — search for the words you want to change and edit them
  directly. Each section is marked with a comment banner like
  `<!-- =============== OUR TREES =============== -->`.
- **Colors** — defined once at the top of the `<style>` block in the `:root`
  section (`--evergreen`, `--red`, `--ice`, etc.). Change a value there and it
  updates everywhere.
- **Opening date / hours** — appear in four places: the red info strip under the
  hero, the "Plan your visit" section, the contact sidebar, and the footer.
  Search for `November 27` and `9–4` to find them all.
- **Images** — drop a new optimized JPEG into `images/` and update the matching
  `<img src="images/…">` (or the hero's `background` in the CSS). Keep images
  at ~1600px wide max and JPEG quality ~80 so the page stays fast.

## The contact form (Formspree)

The contact form is connected to [Formspree](https://formspree.io) (form ID
`mykrkpyn`) and delivers submissions to hoppytreeroh@gmail.com. Visitors see a
thank-you message on the page after sending.

- To see past submissions or change settings, log in at formspree.io with
  hoppytreeroh@gmail.com.
- The free plan includes 50 messages per month.
- If you ever create a new form, update the ID in the form's `action`
  attribute in `index.html` (search for `formspree.io/f/`).

## Publishing

Any static host works: Netlify Drop, Vercel, GitHub Pages, or your registrar's
hosting. Upload `index.html` and the `images/` folder together — that's the
whole site.
