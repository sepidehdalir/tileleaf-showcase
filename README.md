# Tileleaf: Poster Printing

<img src="docs/assets/icon.png" alt="Tileleaf's continuous leaf across four paper tiles" width="160">

**Small sheets. Bigger ideas.**

Tileleaf turns a chosen picture or PDF page into physically sized, numbered A4 or US Letter tiles, with an assembly guide, a printable scale check and matching replacement sheets.

**Status — October 19, 2026:** Version1.0(build1) and Lifetime Pro submitted together at4:41PM PDT; both Waiting for Review. V1 is frozen. iPhone/iPad native workflows and local StoreKit checks passed; the publisher reports device purchase/restore and the requested physical print test working. Exact paper measurements and purchase environment were not supplied. Manual release after approval; not publicly available. TestFlight skipped by publisher instruction.

## One focused workflow

- Choose an image or one page of a supported PDF.
- Set artwork width/height in millimeters, paper orientation, printer margins and overlap.
- Inspect a numbered assembly plan before exporting the labeled PDF.
- Print the guide at actual size and measure its 50 mm square before assembly.
- With Lifetime Pro, save local projects and regenerate selected tiles with stable IDs and source/layout identity.

Complete posters up to four artwork tiles are free, including the guide. A one-time Lifetime Pro purchase adds larger bounded grids, local projects and selected-tile reprints. No subscription; localized pricing comes from Apple.

## Engineering

Native SwiftUI, UIKit, PDFKit, Core Graphics, ImageIO, CryptoKit and StoreKit 2. Universal iPhone/iPad, deployment iOS/iPadOS 15.0. UI adapts to a separate inspector and assembly workspace on larger iPads. Availability compilation is distinct from executed runtime coverage; iOS 17 is the oldest runtime executed so far.

The independent engine computes physical millimeter coordinates, overlap and nondivisible edge regions before converting to PDF points. Replacement page content was independently verified byte-identical to the original tile. Native test evidence covers source orientation, PDF page rotation/crop, transparency, malformed/encrypted files, atomic project recovery and verified local purchase/refund behavior. Local Xcode StoreKit tests do not establish genuine Sandbox or production purchases.

Sources are normalized on-device to at most 4,096 pixels. Limits include 40 MB imports, supported unencrypted PDFs up to 100 pages, at most 100 artwork tiles, and 30 local projects. PDF pages are flattened; this is a home-print workflow without printer drivers or professional color-management claims. Printing paths can scale output; check the printed guide square at actual size before assembly. The publisher confirmed the requested physical print test works; numerical measurements were not supplied.

## Privacy

No account, backend, content upload, advertising or analytics SDK. Native pickers expose selected files; Files providers may download what the user selects. Saved projects remain in protected app storage and may be included in system device backups. Apple handles purchases; the user controls export and print destinations. [Privacy policy](https://sepidehdalir.github.io/tileleaf-showcase/privacy.html) · [Support](https://sepidehdalir.github.io/tileleaf-showcase/support.html).

Commercial source and dated QA evidence are maintained in a separate private repository. This public showcase contains no commercial source, signing material, credentials or user content. The campaign uses reviewed native app captures, original botanical sample artwork and actual PDF exports. Paid features are labeled Lifetime Pro; no generated or reconstructed UI is used.

## App Store campaign

Separate iPhone and iPad compositions show the main value, sizing workflow, PDF guide, selected replacements and local projects.

![Tileleaf iPhone campaign](docs/assets/iphone-campaign.jpg)

![Tileleaf iPad campaign](docs/assets/ipad-campaign.jpg)

Built by **Sepideh Javanbakht Dalir** · [arvinify.com](https://www.arvinify.com) · [hello@arvinify.com](mailto:hello@arvinify.com)
