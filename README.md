# happy birthday sivalia 🎀

A ten-slide, mobile-first birthday site. 13 October 2026.

Tap through: landing → words → photo wall → constellation → the save
counter → polaroid line → looping video → words → the age ceremony →
the button that does the thing.

## Running it

It is plain HTML, CSS and JavaScript. No build step, no dependencies,
no install. Open `index.html`, or serve the folder:

    npx http-server . -p 8080

With GitHub Pages pointed at this repo's default branch, it serves at
the repo URL directly.

`standalone-offline.html` is the entire site — photos, video and music
inlined — as a single file. It needs no server and no network at all.
Useful for sending the site to someone directly.

## Layout

    index.html              the whole site
    assets/img/             10 photos (1–10) + square thumbs (t1–t10)
    assets/video/           the looping clip, mp4 + webm, silent
    assets/audio/           the background track (see its README)

## Notes

- The music starts on the first tap. Every mobile browser blocks audio
  before a user gesture; that is a platform rule, not a bug.
- The video has had its audio stream removed entirely.
- Two video formats are shipped so each browser downloads only the one
  it can decode. Phones take the mp4.
