# Photo Showcase

A simple HTML project that displays a small gallery of animal photos
along with a short descriptive caption for each image, plus a sample
video. This project is part of the
[roadmap.sh](https://roadmap.sh/projects/photo-showcase) front-end
learning path.

## Project Reference

- Roadmap.sh project page:
  https://roadmap.sh/projects/photo-showcase

## Overview

The goal of this project is to practice and demonstrate the use of
core HTML elements for building a media-rich page:

- Semantic page structure (`header`, `main`, `footer`)
- Grouping media with captions using `figure` / `figcaption`
- Embedding images with proper `alt` text for accessibility
- Embedding video with `controls` and a `poster` image
- Providing fallback content for unsupported browsers

## Project Structure

```

photo-showcase/
├── gallery.html
├── README.md
└── assets/
    ├── images/
    │   ├── cat.png
    │   ├── koala.jpeg
    │   ├── turtle.jpeg
    │   ├── racon.jpeg
    │   ├── monky.jpeg
    │   ├── mouse.jpeg
    │   └── DirinDirin.png
    └── videos/
        └── iron-way.mp4

```

> **Note:** In the current `gallery.html`, asset paths are referenced as
> `./images/...` and `./videos/...`. You can either keep that layout or
> move assets into an `assets/` folder as shown above.

## Features

- **Semantic layout** — `header`, `main`, and `footer` are used to
  describe the page regions.
- **Captioned figures** — The first three images use `figure` and
  `figcaption` to pair each photo with a short description.
- **Video player** — A `<video>` element with `controls` and a
  `poster` image, plus fallback text for older browsers.
- **Responsive viewport** — The `meta viewport` tag ensures proper
  scaling on mobile devices.

## Known Issues / Areas for Improvement

These are intentional or known limitations of the current version,
and are good next steps for learning:

1. **Inline sizing with units** — `width="80px"` and `height="80px"`
   should be written without units in HTML, or better, moved to CSS.
2. **Incorrect / missing `alt` text** — The koala image uses
   `alt="cat"`, and one of the raccoon images has an empty `alt`.
3. **No CSS** — The page currently relies on the browser's default
   styles. Adding a `style.css` with a grid or flex layout would
   greatly improve the gallery's appearance.
4. **Inconsistent layout** — Images have different sizes (70px, 80px,
   100px) and only some are wrapped in `figure`.
5. **Duplicate image** — `racon.jpeg` is used twice.
6. **Video accessibility** — No `<track>` element is provided for
   captions or subtitles.
7. **No page metadata** — The `<head>` lacks a `description`, favicon,
   and any linked stylesheet.

## How to Run

1. Clone or download this repository.
2. Make sure the `images/` and `videos/` folders exist next to
   `gallery.html` and contain the referenced files.
3. Open `gallery.html` directly in any modern browser
   (Chrome, Firefox, Safari, Edge).

No build step or server is required.

## Suggested Next Steps

- [ ] Move all `width`/`height` attributes into a CSS file.
- [ ] Fix the incorrect `alt` attributes and fill in the missing ones.
- [ ] Wrap every image in a `figure` + `figcaption` pair.
- [ ] Add a CSS grid to lay out the gallery uniformly.
- [ ] Remove the duplicate raccoon image.
- [ ] Add `<track kind="captions">` to the video.
- [ ] Add a `description` meta tag and a favicon.

## License

This project is for learning purposes. Feel free to reuse and adapt.