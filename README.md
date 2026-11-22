# XAerova — SkyMind demo

A simple, mobile-friendly French demo page. Click Play to watch the complete
2-minute-52-second video with sound. No account or installation is required.

## Publish with GitHub and Cloudflare Pages

1. Unzip this package.
2. Create a GitHub repository and upload **all four files** from the package:
   `index.html`, `demo.mp4`, `poster.jpg`, and `_headers`. Keep them together at
   the repository root, without renaming them. Do not upload the ZIP itself.
3. In Cloudflare, open **Workers & Pages**, create a **Pages** project, choose
   **Import an existing Git repository**, and select that repository.
4. Use the following settings:

   | Setting | Value |
   | --- | --- |
   | Production branch | `main` (or your repository's actual branch) |
   | Framework preset | None |
   | Build command | `exit 0` |
   | Build output directory | `/` (repository root) |

5. Deploy, open the resulting `https://…pages.dev` address, and press Play.
   Share that page address with the competition organizers.

The HTML includes its own styling, fonts and logo. The MP4 and poster must stay
beside it. The site works without a backend, third-party video host or JavaScript
framework. JavaScript adds the large Play button; the native video controls also
work without it.

## Video

The supplied video was remuxed for progressive browser playback, without
re-encoding its picture or sound. It retains its original portrait frame,
including any black bars already present in the video. It uses H.264 video and
AAC audio and is approximately 18.4 MB, below the 25 MiB per-file limit on Pages.

To replace it, use a browser-compatible MP4 named `demo.mp4` and update the
displayed duration in `index.html` if necessary. Choose a new still image named
`poster.jpg` if desired.

## References

- Cloudflare static HTML: https://developers.cloudflare.com/pages/framework-guides/deploy-anything/
- Cloudflare Pages limits: https://developers.cloudflare.com/pages/platform/limits/

This package is ready to deploy; it does not itself create a public URL.
