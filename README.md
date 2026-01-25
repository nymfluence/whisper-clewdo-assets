# whisper-clewdo-assets

Static image assets for WHISPER · CLEWDO.

## Folder layout

- `clewdo/rooms/`  
  Contains the base room images in sequence, named:
  `01-entrance-hall-base.png` … `36-vip-lounge-base.png`

- `clewdo/manifest.json`  
  Room metadata + avatar slot coordinates for dynamic image generation.

## How rendering works (important)

The base room images already contain:
- the victim Polaroid with a **blank black 1:1 frame**
- the killer Polaroid with a **red question mark**

Therefore, the image generator must ONLY:
- paste the eliminated player’s avatar into the blank black square at `(x,y)`
- using a consistent square size (`defaultAvatarSize`)

No polaroid overlays are required.
