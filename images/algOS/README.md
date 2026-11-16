# algOS final artwork

Algorant selected the 40% size, then the medium corner radius for the O ("medium radius, the 4px"). These are reusable wordmark assets, not an operating-system distribution or installed desktop branding.

Showroom selection: Algorant chose "medium radius, the 4px" and patina green. The README uses the medium-radius patina dark/light pair. Square marks are exported, but no avatar has been applied; that is a separate later choice.

## Selection and provenance

- Selected corner rounding: **medium, radius 0.45 cell** of the 15×15 O grid (4.17 px on the 1280 banner), chosen on the patina banner from the rounded-O comparison mockups. It is applied to all four colours, dark and light (8 contexts).
- Every contour vertex gets the same radius: outer and inner convex corners, and concave corners (a fillet that fills the corner). Straight 1-cell strokes, the maze topology, palette, text, layout and icon tiles are unchanged. Two-tone keeps its hard, straight ochre/patina boundaries.
- Filenames are identical to the earlier sharp-cornered set, so this bundle is a complete replacement.

## Geometry and sizing

The O is the standard `apps/fastfetch/logos/omarchy-mark.svg` 15×15 rect geometry (95 filled cells), recolored and with rounded corners. Two-tone retains the original filled-cell layout as an ochre outer frame and patina interior; the rounded contour softens corner coverage only. All four wordmarks share the same cap and alignment. The 1280-pixel PNGs render a 57 px lowercase body against a 143–144 px OS cap (0.396–0.399 across light/dark contexts; approximately 40%). The SVG design cap is 142 units; O is 98% of that cap.

Palette: blue/aqua `#83a598`, patina `#689d6a`, ochre `#e6bf86`, two-tone ochre + patina. Dark banners use `#151a19` with vellum text `#ebdbb2`; light banners use vellum `#ebdbb2` with ashbronze text `#665c54`. Icons have dark ash-green or vellum tiles.

## How the pixels were made

- At the smallest icon sizes, the pixel-grid radius is limited to half the shorter adjacent edge so tiny fillets do not overlap; the selected vector radius remains 0.45 cell.
- Each PNG's O is rasterised from vector at the target size, with the straight edges snapped to the pixel grid exactly as the approved crisp renders were (at that size's own grid, so 2560 and the icon sizes are not upscaled 1280/1024 rasters). Rounded corners are anti-aliased.
- Every pixel outside the O is the approved original pixel, including text, background and the icon tile's shape and alpha. Only pixels at the O's corners differ from the sharp set.
- The sharp rebuild of the O matched the approved PNGs pixel for pixel in all 8 contexts at every size (1280, 2560 and 1024–16 icons). At 16 and 32 px a 0.45-cell radius is under 1 px, so those icons differ from the sharp set only by faint anti-aliasing at the corners.
- The SVG masters draw the O as a path in pixel-snapped 1280 banner coordinates: they render exactly to the 1280 PNG. At other sizes they scale as ordinary vector art (the O is then a scaled copy of the 1280 geometry, not re-snapped; the 2560 PNG is the natively snapped one).

## Font portability

The SVG masters retain editable text and require **JetBrainsMono Nerd Font Regular**, the installed Nerd-Font-patched JetBrains Mono face (`/usr/share/fonts/TTF/JetBrainsMonoNerdFont-Regular.ttf`). The existing render toolchain has no text-to-path converter, so the font dependency is documented rather than faked. PNGs are already rasterized and font-independent.

## Files

- 8 SVG masters: `algOS-<color>-<dark|light>.svg`.
- 16 banner PNGs: `algOS-<color>-<dark|light>-<1280|2560>.png` (1280×360 or 2560×720).
- 56 square-icon PNGs: `icon-<color>-<dark|light>-<size>.png`; each color/context has 1024, 512, 256, 64, 48, 32 and 16 px exports.
- This README: 81 files in total. No generators or scripts are in this folder.
