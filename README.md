# Image Assets for the Herbs App

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/suradet-ps/herbs-app-images/issues)

---

## ◆ PULSE

A formulary without pictures is a list of names; with them, it is a
recognition. This repository is the version-controlled image shelf for
the [herbs-app](https://github.com/suradet-ps/herbs-app): every
herb's photograph, publicly accessible, fetched by the app at runtime
and keyed through the `ImageUrl` column of the Google Sheet. One repo
per purpose, one image per herb, and a naming convention the app can
depend on.

| Public ▣ | Raw URLs ▣ | Versioned ▣ | Convention ▣ |
|---|---|---|---|

*The shelf - host, reference, serve - is sealed.*

> Maintained by **suradet-ps** - the images the formulary shows
> are the images this repository holds.
>
> **suradet-ps**, artifact keeper

---

## ◆ IGNITION

No install, no build - a browser and a raw URL.

```
⟫ git clone https://github.com/suradet-ps/herbs-app-images.git
```

An image is referenced through the raw URL, not the GitHub preview
page:

```
https://raw.githubusercontent.com/suradet-ps/<repo>/main/<image_name.png>
```

That URL is what lands in the `ImageUrl` column of the Google Sheet -
right-click the image, copy the image address, paste.

<details>
<summary>Adding an image</summary>

1. `Add file` > `Upload files` in the repo.
2. Drag and drop; commit with a descriptive message.
3. Name it by the convention: lowercase, hyphen-separated, descriptive
   (`holy-basil.jpg`, never `Holy Basil.jpg`).

</details>

---

## ◆ ANATOMY

One shelf, one convention, no code in the way.

- **Hosts** - every herb image lives in this repository, publicly
  accessible, version-controlled - the app's pictures have the same
  history discipline as its code.
- **Serves** - the app fetches each image at runtime through the raw
  URL stored in the Google Sheet - add a picture to the repo, put the
  URL in the sheet, and the formulary shows it.
- **Names** - lowercase, hyphen-separated, descriptive: the naming
  convention keeps URLs stable and predictable - what the sheet
  points to is what the repo holds.
- **Grows** - images sit at the root for now; categories can earn
  subdirectories when the shelf outgrows the flat floor.

---

## ◆ RITUALS

**The core ceremony** - adding a herb's picture:

1. Upload the image with a descriptive commit message.
2. Verify the raw URL resolves - right-click, copy, paste into a
   browser first.
3. Paste the URL into the herb's `ImageUrl` cell in the Google Sheet.
4. Refresh the app; the formulary now shows what the herb is.

**The ceremony of the raw URL** - the preview page is for humans; the
`raw.githubusercontent.com` address is for `<img>` tags. The
distinction is written into the workflow so the sheet never points at
a page instead of a picture.

**The ceremony of the stable name** - a lowercase, hyphenated name
survives browsers, filesystems, and future references. The URL you
commit today is the URL the sheet can still resolve next year.

---

## ◆ ECHOES

**Where this artifact is heading**

```
host    ▸ public, version-controlled image shelf ────────────────────── ▸ sealed
serve   ▸ raw URLs consumed by the app at runtime ──────────────────── ▸ sealed
name    ▸ lowercase hyphen-separated convention ─────────────────────── ▸ sealed
grow    ▸ subdirectories when the collection earns them ─────────────── ▸ open
```

**Raising the artifact** - the convention lives in the README, the
images in the root. Open an issue first to discuss a change.

**Status** - the shelf is active and feeding the formulary.

> Ensure you have the rights to every image you upload - the
> collection is intended for use within the associated project.

---

```
  ─────────────────────────────────────────
   A herb named is known.
   A herb pictured is recognized.
  ─────────────────────────────────────────
```

Open source under the [MIT License](LICENSE).