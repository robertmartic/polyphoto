# PolyPhoto

PolyPhoto 0.6.0 is a local Windows photo editor. All current tools are free and unlocked.

[Download the Windows installer](https://downloads.polystudio.tools/polyphoto/0.6.0/PolyPhoto-0.6.0-setup.exe) or [portable ZIP](https://downloads.polystudio.tools/polyphoto/0.6.0/PolyPhoto-0.6.0-win-x64.zip).

Open PNG/JPEG images and .polyphoto projects in independent document tabs. Edit raster layers, groups, masks, blends and adjustment layers. Export a flattened PNG, JPEG or lossless WebP copy without changing the original project.

Use Brush, Eraser, Clone Stamp, Paint Bucket, Healing Brush, Red Eye and Eyedropper. Selections support rectangles, ellipses, freehand, add/subtract and movement with live preview. Crop, image/canvas resize, rotate, flip and interactive transforms are above the canvas.

Add editable text with Ubuntu or Hack, size, color and multiline alignment. Reopen it using Edit text in the layer controls. Use Move (K) to drag it; Text / Move arrow keys nudge 1 px, Shift+arrows 10 px. Rasterize text explicitly before painting or free transforms; Undo restores the editable layer.

Adjust includes Tone, Levels, Curves, Hue / Saturation, Color Balance, Exposure, Temperature / Tint and Vibrance. Adjustment layers stay editable, support opacity and masks, and offer Show before. Healing Brush (J) adapts source texture to local color: Alt+click a source on the active raster layer, then paint. Red Eye (R) reduces red-dominant pixels. Size, Hardness and Opacity control retouching.

Export remembers format, JPEG quality/background and original/custom dimensions. Estimate file size uses the same encoder as export. PNG and WebP preserve transparency; JPEG is lossy and uses the chosen background. WebP export is lossless; opening WebP is not yet supported.

Keyboard: Ctrl+N/O/S, Ctrl+Shift+S, Ctrl+Alt+S Save all, Ctrl+Z/Y, Ctrl+C/V images, Ctrl+A/D, Ctrl+Shift+I invert, Ctrl+J copy selection, Delete; M Select, K Move, B Brush, E Eraser, S Clone Stamp, J Healing Brush, R Red Eye, T Text, G Bucket, I Eyedropper, H Hand, V or Ctrl+T Transform, F1 Help. Text fields retain normal typing and paste. Space/middle mouse pans; Ctrl+wheel zooms.

Projects preserve layers, hidden RGB, masks, groups and editable adjustments/text. Formats 1–4 remain readable. Text and new adjustments require format 5 and PolyPhoto 0.6.0 or later; projects without them keep their earlier format. Undo, current selection and clone anchors are temporary state. Recovery encrypts checkpoints after 30 seconds without edits; it is tied to the Windows account and machine and is not a backup. Edits after the last completed checkpoint can be lost.

Limits: 24 million pixels, 16,384 px per side, 256 MiB input, 16 layers and 512 MiB padded pixel/mask storage per document, 16 tabs and a shared 2 GiB pixel/history budget (not a process working-set cap). Undo keeps changed blocks within 256 MiB; older steps are trimmed. Text supports two bundled fonts, up to 2,048 characters, 128 lines and 512 px font size. Complex-script shaping, arbitrary installed fonts and automatic line wrapping are not supported. Healing is source-based local color matching, without content-aware object removal. Moved previews are downsampled to at most 1,024 px per side; final pixels retain full resolution.

Unsupported: animation, RAW, PSD, XCF, CMYK, HDR, 16/32-bit channels and multi-page images. ICC profiles are converted to sRGB on accepted import; unsupported profiles require the explicit Open as sRGB override. EXIF orientation is applied; other EXIF/IPTC/XMP metadata, including GPS, is omitted from projects and exports. Off-canvas pixel content is clipped by applied transforms. Compression is checked for cancellation before and after encoding, not inside the codec.

Choose Help for searchable offline instructions. Updates use the signed [PolyStudio channel](https://updates.polystudio.tools/polyphoto/stable.json) and verified official downloads. GitHub 0.2.9 remains a transition for older clients. See [installation](docs/INSTALLATION.md), [updates](docs/UPDATES.md), the [changelog](CHANGELOG.md), software terms and third-party notices.
