# PolyPhoto

![PolyPhoto](assets/polyphoto.png)

Version 0.1.5. A standalone local raster editor for Windows x64. English interface, light/dark themes, free and unlocked. No account, photo upload, subscription or activation.

[Download PolyPhoto for Windows](https://github.com/robertmartic/polyphoto/releases/latest). Choose the -setup.exe asset for installation or the -win-x64.zip asset for portable use. Official updates use this same public release channel.

File and operation commands use local vector icons. Raster tools stay in a vertical selector with a persistent active indicator. Narrow toolbars move commands into More; use Down to enter and Escape to close it. Tooltips include existing shortcuts and commands expose accessible names in both themes.

Create an image, or open a still PNG/JPEG as a new unsaved project. Save and Save as use the versioned .polyphoto format. Export creates a PNG/JPEG copy and does not mark the project saved. The original imported image is never automatically overwritten.

Raster layers with names, visibility, opacity and ordering; 8-bit channels, sRGB. Projects retain every layer, including hidden pixels. Format 1 projects remain readable; format 2 projects require PolyPhoto 0.1.5 or newer. Embedded ICC profiles are converted only after the import notice is accepted. Unsupported profiles stop import, with an explicit option to ignore the profile and assume sRGB. EXIF orientation is applied once. Other EXIF/IPTC/XMP metadata, including GPS, is not copied into projects/exports. PNG keeps transparency; JPEG uses the selected background and quality with lossy compression.

Limits: 24 million pixels; 16,384 pixels per side; 256 MiB input file; up to 16 layers within a 512 MiB padded pixel-storage limit; one document per window. Unsupported: animation, CMYK, HDR, 16/32-bit channels, RAW, PSD, XCF and multi-page images. Undo retains changed pixel blocks within a 256 MiB history budget. Older history is removed when needed. Undo is not saved in projects.

Tools: rectangular selection, selection delete/crop, round brush/eraser with size and opacity, color picker/eyedropper, separate image/canvas resize, 90-degree rotations, flips and brightness/contrast. A completed stroke or applied operation is one Undo step. Selection changes can also be undone. Add, duplicate, rename, reorder, hide and remove layers in the Layers panel. Brush, eraser, selection delete and brightness/contrast affect the active layer. Image crop/resize/rotate/flip affect the entire stack. Import PNG/JPEG as a layer at the top left; pixels beyond the canvas are clipped. Transform layer previews movement, uniform scale, arbitrary rotation and mirroring with Apply/Cancel. Scaling/rotation use the canvas center; Apply clips off-canvas content and Undo restores it. Choose bilinear interpolation for photos or nearest neighbour for pixel art. PNG/JPEG exports flatten visible layers with opacity. Advanced selections, moving selections, clipboard and text are planned separately.

Keyboard: Ctrl+N/O/S, Ctrl+Shift+S, Ctrl+Z/Y, Ctrl+A/D, Delete; B brush, E eraser, M rectangle, I eyedropper, H pan, V transform layer. Hold Space or use the middle mouse button to pan. Ctrl+wheel zooms. Fit follows window size; 100% maps image pixels to physical display pixels.

Recovery writes changed encrypted blocks after 30 seconds without edits. A busy operation postpones it. Recovery is tied to this Windows account and machine; it is not a backup. Restore opens an unsaved copy. Saving, or explicitly discarding/closing the document, removes its checkpoint. Edits since the last completed checkpoint can be lost.

See docs/INSTALLATION.md and docs/UPDATES.md. Software terms and third-party notices are included.
