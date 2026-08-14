# LFP Connect brand assets

A deliberately simple identity for [lfpconnect.io](https://lfpconnect.io): a stylized lowercase `lfp` monogram in signature coral, paired with a clean `connect` wordmark.

## Quick use

- Primary transparent wordmark: `assets/svg/lfp-connect.svg`
- Reversed transparent wordmark: `assets/svg/lfp-connect-reversed.svg`
- Theme-aware transparent wordmark: `assets/svg/lfp-connect-auto.svg`
- Light presentation tile: `assets/svg/lfp-light.svg`
- Dark presentation tile: `assets/svg/lfp-dark.svg`
- Compact transparent monogram: `assets/svg/lfp-coral.svg`
- Favicon/app icon: `assets/svg/lfp-favicon.svg`
- Generated presentation boards: `assets/brandboards/`
- Authentik theme and flat flow background: `assets/authentik/`
- CSS and JSON design tokens: `tokens/`

### Composable product lockups

Use `assets/svg/lfp-coral.svg` as the fixed `lfp` monogram, then render the
lowercase product name as live text beside it. The reference wordmark family is
Inter Variable at weight 520 with `-0.026em` tracking; equivalent CSS tokens
live in `tokens/brand.css`. This keeps product names such as `connect`, `pipe`,
or `admin` editable and accessible without converting them to SVG paths.

Load Inter Variable in the consuming application so the lockup does not depend
on fonts installed on the host. Keep the suffix lowercase and align its visual
baseline to the monogram rather than vertically centering its bounding box.

The SVG files are the production source of truth. The generated PNG boards are visual references, not masters.

## Palette

| Token | Hex | Use |
| --- | --- | --- |
| Coral | `#FF6F61` | Primary identity |
| Coral hover | `#E85C50` | Interactive state |
| Ink | `#0B1426` | Dark background and text |
| Warm white | `#FFF9F5` | Light background |
| Soft coral | `#FFF0EC` | Subtle surfaces |

## Rules

- Keep the logo lowercase.
- Use coral as a solid fill; do not apply gradients, shadows, or outlines.
- Leave clear space equal to roughly half the logo height.
- Use the full `lfp connect` wordmark for headers and identity surfaces.
- Use the compact `lfp` monogram for favicons, app icons, and very small spaces.
- Prefer warm white or ink backgrounds.

## License

Copyright © LFP Connect. See [LICENSE](LICENSE).
