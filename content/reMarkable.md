# reMarkable

The reMarkable is an e-ink-based tablet meant for reading and writing.

  * Reading and annotating PDFs on the beach is really amazing. This is the high-order bit.

![](EBC2E7F5-F633-47CD-9CBA-D4F459350B27_1_105_c.jpeg)

  * It’s wonderful to be able to read and annotate full-page PDFs rather than EPUBs.
  * The device incredibly slow, exacerbating [[Poor performance disrupts nonlinear reading in digital reading]]
  * The workflow for doing anything with annotations made on-device is abysmal. On-device, one can’t search or quickly navigate among them. On a computer, they’re simply flattened into the PDF. And there’s no automatic syncing whatsoever. Shockingly bad.
  * The EPUB reader implementation is truly awful: incredibly slow, painful navigation, etc.
  * Getting books onto it requires breaking using a computer and breaking DRM.
  * The form factor’s great: light, a good size, good materials.
  * Poor but tolerable battery life.
  * Quite expensive at $500… but was discounted to $279 in May 2020! I returned mine but bought another at the lower price.

## Syncing

I’d like very much to sync my on-disk library with the reMarkable. I imagine I’ll have to set aside a day or two and just build that functionality.

There’s a Typescript implementation of the cloud API: [[reMarkable- typescript/src at master · Ogdentrod/reMarkable-typescript · GitHub]]

Documentation of the API here: [[Storage · splitbrain/ReMarkableAPI Wiki · GitHub]]

Once I download the lines files, I can convert them to SVG using this script: [[maxio/rm_tools at master · lschwetlick/maxio · GitHub]]

Q. Valuation as of May 2022? A. $1B

Q. Devices sold as of May 2022? A. 1M
