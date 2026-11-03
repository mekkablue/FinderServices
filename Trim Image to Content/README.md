# Trim Image to Content

A Finder Quick Action that trims images to their content. The color of the top left pixel counts as background; the smallest rectangle that keeps every differing pixel is cropped out. If the top left pixel is fully transparent, all fully transparent pixels count as background.

The result is saved as `<name> trimmed.<ext>` next to the original, which is never overwritten. Animated (multi-frame) images are skipped. The match is exact, so lossy formats like JPEG may trim less than expected where compression noise touches the edge.

## Install

```bash
./install.sh
```

Then right-click an image in Finder > Quick Actions > Trim Image to Content. You may have to enable it in System Settings > Extensions > Finder.

Requires Python 3 with Pillow (`pip3 install Pillow`).

## Develop

`trim_image.py` is the source. After editing it, run `python3 build_workflow.py` to regenerate the self-contained `.workflow`.
