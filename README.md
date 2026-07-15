# CLUB69 OpenWorld Banners

Public delivery repository for the remote banner atlases used by the CLUB69 OpenWorld VRChat world.

The protected administration interface is hosted separately. This repository contains public delivery assets only.

## Stable public atlas URLs

| Atlas | Grid | Frame size | Live surfaces | Direct URL |
| --- | --- | --- | ---: | --- |
| Horizontal Atlas | 2 columns x 4 rows | 1024 x 512 | 3 | https://club69megumin.github.io/club69-banners-openworld/banners/horizontal-atlas.jpg |
| Vertical Main Atlas | 4 columns x 2 rows | 512 x 1024 | 1 | https://club69megumin.github.io/club69-banners-openworld/banners/vertical-main-atlas.jpg |
| Vertical Atlas | 4 columns x 2 rows | 512 x 1024 | 3 | https://club69megumin.github.io/club69-banners-openworld/banners/vertical-atlas.jpg |

The three atlas downloads feed seven live banner surfaces. Sharing one downloaded texture across each material group avoids duplicate 2048 x 2048 downloads in VRChat.

## Publishing rules

- Keep all three filenames stable and replace their contents atomically.
- Every atlas must remain exactly **2048 x 2048 pixels**.
- Every atlas contains eight frames. Do not change its grid, cell order, or orientation.
- Use optimized JPEG images in the sRGB color space.
- Keep texture wrapping set to **Repeat** in Unity so the existing atlas animations continue to work.
- Publish only final images intended to be visible to every visitor.
- Never commit passwords, API tokens, server configuration, private source files, or personal data.

The retired per-surface placeholder files are intentionally no longer part of the delivery contract.

## Files

- `banners/`: The three stable 2048 x 2048 atlases consumed by VRChat.
- `banner-manifest.json`: Machine-readable atlas, grid, and surface metadata.
- `index.html`: Public atlas preview and delivery status page.
