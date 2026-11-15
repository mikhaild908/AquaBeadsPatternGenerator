# Aquabeads Pattern Generator

Convert any image into an Aquabeads-style bead pattern using a hexagonal bead grid. The application runs entirely in the browser and requires no server, database, or installation.

## Features

- Upload JPG, PNG, WEBP, and other browser-supported image formats
- Convert images to an 8-bit color palette before bead generation
- Optional Floyd-Steinberg dithering for smoother gradients
- Automatic color matching to an Aquabeads-inspired palette
- Hexagonal bead layout similar to real Aquabeads trays
- Adjustable board dimensions
- Adjustable bead size
- Adjustable color depth (8-256 colors)
- Real-time pattern generation
- Bead inventory/count breakdown by color
- Download completed pattern as PNG
- 100% client-side processing

---

## Screenshot

Recommended workflow:

1. Upload an image
2. Resize to desired board dimensions
3. Adjust color depth
4. Enable or disable dithering
5. Review bead counts
6. Download the finished pattern

---

## How It Works

The application converts an uploaded image into an Aquabeads pattern using the following pipeline:

```text
Original Image
      ↓
Resize to Board Size
      ↓
8-Bit Color Quantization
      ↓
Optional Dithering
      ↓
Aquabeads Color Mapping
      ↓
Hexagonal Bead Grid Rendering
      ↓
Bead Inventory Calculation
```

---

## Requirements

### Browser Support

Modern browsers including:

- Microsoft Edge
- Google Chrome
- Mozilla Firefox
- Safari

### No Dependencies

The project uses:

- HTML5
- CSS3
- Vanilla JavaScript
- Canvas API

No frameworks or external libraries are required.

---

## Installation

Clone or download the repository:

```bash
git clone https://github.com/yourusername/aquabeads-pattern-generator.git
```

Open the HTML file:

```bash
aquabeads-generator.html
```

or simply double-click the file in your file explorer.

---

## Usage

### Upload an Image

Click the **Image** selector and choose a file from your computer.

### Set Board Dimensions

Choose the desired bead board size.

Examples:

| Board Size | Usage |
|------------|---------|
| 20 × 20 | Small icons |
| 40 × 40 | Character sprites |
| 50 × 50 | Standard artwork |
| 80 × 80 | Detailed images |

### Select Color Depth

Lower values:

- Simpler patterns
- Fewer bead colors
- Faster assembly

Higher values:

- Better image quality
- More bead colors
- More realistic results

Recommended values:

```text
32-64 Colors
```

### Toggle Dithering

Dithering helps smooth gradients and transitions.

Best for:

- Photographs
- Anime artwork
- Landscapes
- Pet photos

May be disabled for:

- Pixel art
- Logos
- Simple illustrations

### Download Pattern

Click **Download PNG** to save the generated bead pattern.

---

## Project Structure

```text
aquabeads-pattern-generator/
│
├── aquabeads-generator.html
├── README.md
│
└── assets/
    ├── screenshots/
    └── examples/
```

---

## Aquabeads Palette

The included palette uses approximate Aquabeads-compatible colors such as:

- White
- Black
- Yellow
- Orange
- Red
- Pink
- Purple
- Blue
- Light Blue
- Green
- Brown
- Gray

and additional shades commonly found in Aquabeads refill packs.

Future versions may support:

- Official Aquabeads color IDs
- Aquabeads color numbers
- Custom color packs
- Palette extraction from official color charts

---

## Future Improvements

### Planned Features

- Official Aquabeads color chart support
- Bead color numbers (e.g. 4-01, 4-02)
- Printable instruction sheets
- Multi-page poster patterns
- PDF export
- Background removal
- Image cropping tool
- Symbol-based color patterns
- Inventory management
- Missing bead detection
- Custom Aquabeads palettes
- Heart and star-shaped board layouts
- Pegboard-specific templates

---

## Performance Notes

Large board sizes can increase processing time.

Recommended maximum:

```text
100 × 100 beads
```

for smooth performance on most computers.

---

## Troubleshooting

### Image Doesn't Appear

Ensure:

- The image format is supported
- The file is not corrupted
- JavaScript is enabled

### Pattern Looks Too Detailed

Try:

- Lowering color depth
- Reducing board size
- Disabling dithering

### Pattern Looks Too Simple

Try:

- Increasing color depth
- Increasing board dimensions
- Enabling dithering

---

## Development

The application is built using:

```text
HTML5 Canvas
CSS3
Vanilla JavaScript
```

Main rendering steps:

1. Resize image
2. Quantize to 8-bit color
3. Apply optional dithering
4. Convert to Aquabeads palette
5. Render hexagonal bead pattern
6. Aggregate bead counts

---

## License

MIT License

You are free to use, modify, and distribute this project.

---

## Acknowledgments

Inspired by the Aquabeads crafting system and traditional bead-pattern design software.

Aquabeads is a trademark of its respective owner. This project is an independent fan-made pattern generator and is not affiliated with or endorsed by Aquabeads or Epoch Company.
