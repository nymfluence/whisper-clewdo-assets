# whisper-clewdo-assets

Asset repository for WHISPER · CLEWDO.

## Folder structure

- `clewdo/rooms/`  
  Base room images (PNG). These already contain:
  - the blank Polaroid window (victim PFP goes here)
  - the killer red question mark Polaroid baked into the image (elimination cards)

- `clewdo/config/pfp-frames.json`  
  Coordinates + dimensions for where to composite the victim PFP into each room template.

- `clewdo/config/rooms.json`  
  Room index mapping and metadata.

## Notes

- Room 01 and 02 do not require victim PFP compositing.
- Rooms 03–35 require victim PFP compositing into the blank Polaroid window.
- Room 36 (VIP Lounge) also requires victim PFP compositing (winner/murdered reveal).

## Raw file usage

When served via GitHub raw URLs, the API can fetch templates and config directly.
