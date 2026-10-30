# toss-share-og

Public 1200x600 Open Graph images for Neo Genesis mini apps on Apps in Toss.
`getTossShareLink(path, ogImageUrl)` (SDK 3: `Share.createLink({ path, ogImageUrl })`) needs an absolute https URL,
and the game source trees are private, so the share previews are served from here:

    https://neogenesisai.github.io/toss-share-og/<appName>.jpg

- `index.json` lists every image (`appName`, mini app ID, title, size, URL).
- `kind: thumbnail` images are the mini app's own approved horizontal thumbnail from the Apps in Toss console, fitted to
  1200x600 without cropping or added text. `kind: provisional-icon` images use the console icon and the app title until a
  horizontal thumbnail is registered.
- All pictures are Neo Genesis's own console images. Nothing here is executed.

Made by `mintlab/shared/growth/tools/make_og.py`. Published by omp-toss-mission (exposure optimization).
