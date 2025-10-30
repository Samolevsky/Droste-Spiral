# Droste Spiral Effect

A powerful web-based image editor that creates mesmerizing Droste spiral effects using WebGL. Transform any image into an infinite recursive spiral with real-time preview and extensive customization options.

![Droste Spiral Effect](https://img.shields.io/badge/WebGL-Powered-blue) ![License](https://img.shields.io/badge/license-MIT-green)

## What is the Droste Effect?

The Droste effect is a recursive visual phenomenon where an image appears within itself in a continuous loop. Named after a Dutch cocoa brand's packaging, this effect creates an infinite spiral that draws the viewer into a hypnotic, self-similar pattern. This application takes the classic Droste effect and adds dynamic spiral transformations for stunning visual results.

## Features

- **Real-time WebGL Rendering** - Instant preview of all changes with hardware-accelerated graphics
- **Flexible Image Import** - Support for JPG, PNG, WebP, GIF, and SVG formats (up to 100MB)
- **Comprehensive Transform Controls** - Fine-tune scale, rotation, and positioning
- **Customizable Repetition** - Control inner recursion levels and outer repetitions
- **Spiral Effect Toggle** - Switch between classic Droste and spiral variations
- **Animation System** - Animate spiral rotation with adjustable speed and direction
- **Boundary Visualization** - Optional boundary overlay with custom colors and thickness
- **High-Resolution Export** - Download PNG images up to 8192×8192 pixels
- **GIF Animation Export** - Create animated GIFs of your spiral effects
- **Dark/Light Theme** - Comfortable viewing in any lighting condition
- **Canvas Zoom & Pan** - Navigate and inspect your creation with precision
- **Keyboard Shortcuts** - Efficient workflow with hotkeys

## Getting Started

### Installation

1. Clone or download this repository
2. Open `index.html` in a modern web browser (Chrome, Firefox, Safari, or Edge)
3. No build process or dependencies required!

### Quick Start

1. **Upload an Image**
   - Click the upload area in the sidebar
   - Drag and drop an image onto the canvas
   - Or press `Ctrl/Cmd+O` to open the file picker

2. **Adjust Parameters**
   - Use the sliders to modify the effect
   - Changes apply in real-time

3. **Export Your Creation**
   - Set your desired output dimensions
   - Click "Download PNG" for a static image
   - Click "Export GIF" for an animated version

## User Guide

### Image Section

**Upload Methods:**
- Click the "Drop image here or click to upload" area
- Drag and drop an image file onto the sidebar or canvas
- Use keyboard shortcut `Ctrl/Cmd+O`

**Supported Formats:** JPG, PNG, WebP, GIF, SVG  
**Maximum File Size:** 100MB

### Transform Controls

#### Scale (0.05 - 0.95)
Controls the size ratio between recursive layers. Lower values create tighter spirals with more visible repetitions, while higher values produce looser, more spread-out effects.

**Recommended Settings:**
- Tight spiral: 0.30 - 0.45
- Balanced: 0.45 - 0.60
- Loose spiral: 0.60 - 0.80

#### Rotation (-180° to 180°)
Rotates each recursive layer relative to the previous one. Creates the characteristic spiral twist of the Droste effect.

**Tips:**
- Small angles (5° - 15°): Subtle spiral
- Medium angles (15° - 45°): Classic spiral look
- Large angles (45° - 90°): Dramatic, twisted effect
- Negative values: Reverse spiral direction

#### Offset X & Y (0.00 - 1.00)
Shifts the center point of the recursive transformation. Use these to position where the spiral converges.

**Default:** 0.50 (centered)  
**Usage:**
- Move the focal point to emphasize specific image areas
- Create off-center spirals for asymmetric compositions
- Combine with rotation for dynamic effects

### Repetition Controls

#### Inner Levels (0 - 64)
Determines how many recursive layers are rendered going inward toward the center.

**Performance Note:** Higher values (>32) may impact performance on slower devices.

**Recommended:**
- Quick preview: 4 - 8
- Standard quality: 8 - 16
- High detail: 16 - 32

#### Outer Repeat (1 - 64)
Controls how many times the pattern repeats outward from the center.

**Usage:**
- 1: Single spiral
- 4 - 8: Balanced coverage
- 16+: Dense, kaleidoscope-like patterns

### Options

#### Spiral Effect
When enabled, applies the characteristic spiral transformation. Disable for a classic concentric Droste effect without rotation.

#### Reverse Order
Reverses the rendering order of layers, changing which layers appear on top. Useful for creating different depth effects.

#### Show Boundary
Displays a colored border around the image boundaries, helpful for:
- Visualizing the transformation area
- Creating framed effects
- Debugging alignment issues

**Boundary Color:** Click the color swatch or enter a hex code  
**Boundary Thickness:** Adjust from 1 to 100 pixels

### Animation

#### Play/Pause Button
Located to the left of "Animation Speed" - click to start or stop the animation.

#### Animation Speed (-2.0 to 2.0)
Controls the rotation speed and direction of the spiral animation.

**Values:**
- 0.0: No animation (static)
- Positive: Clockwise rotation
- Negative: Counter-clockwise rotation
- ±0.5 to ±1.0: Smooth, meditative speed
- ±1.5 to ±2.0: Fast, dynamic motion

**Tip:** Set to 0 when adjusting other parameters for easier preview.

### Output

#### Dimensions
Set the width and height of your exported image.

**Link Button:** Click to lock aspect ratio (maintains proportions when changing one dimension)

**Recommendations:**
- Square dimensions (1024×1024, 2048×2048) work best for symmetrical spirals
- Supported range: 256 to 8192 pixels
- Higher resolutions require more processing time

#### Download PNG
Exports a single frame at the current animation state with your specified dimensions.

#### Export GIF
Creates an animated GIF capturing 1 second of animation at 30 FPS.

**Notes:**
- Animation speed must be non-zero
- GIF export may take 10-30 seconds depending on dimensions
- Progress indicator shows during export
- Recommended dimensions: 512×512 to 1024×1024 for reasonable file sizes

### Canvas Controls

#### Zoom Toolbar
Located at the bottom-right of the canvas:

- **Zoom In (+):** Increase magnification
- **Zoom Out (-):** Decrease magnification
- **Zoom Percentage:** Click to type a custom zoom level
- **Reset:** Return to 100% zoom

**Keyboard Shortcuts:**
- `+` or `=`: Zoom in
- `-`: Zoom out
- `0`: Reset zoom to 100%

#### Pan
Click and drag on the canvas to pan around when zoomed in.

### Theme Toggle
Click the sun/moon icon in the top-right corner to switch between light and dark themes.

## Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl/Cmd+O` | Open image file picker |
| `+` or `=` | Zoom in |
| `-` | Zoom out |
| `0` | Reset zoom to 100% |
| `Space` | Play/Pause animation |

## Tips & Tricks

### Creating Stunning Effects

1. **Start Simple:** Begin with default settings and adjust one parameter at a time
2. **Symmetry Matters:** Use square images and dimensions for the most balanced results
3. **Layer Balance:** Match inner levels with outer repeat for even coverage
4. **Animation Sweet Spot:** Try animation speeds between 0.3 and 0.8 for smooth, watchable loops
5. **Color Boundaries:** Use boundary colors that contrast with your image for striking frames

### Performance Optimization

- Lower inner levels and outer repeat values for smoother real-time preview
- Reduce canvas zoom when adjusting parameters
- Close other browser tabs when exporting high-resolution images
- Use smaller dimensions (512×512 or 1024×1024) for GIF exports

### Creative Ideas

- **Portraits:** Center faces with low scale values for hypnotic eye effects
- **Patterns:** Use geometric or mandala images for kaleidoscope results
- **Nature:** Flowers and spirals create organic, fractal-like compositions
- **Text:** Circular text arrangements create interesting typographic spirals
- **Abstract:** Combine high rotation angles with asymmetric offsets for chaotic beauty

## Technical Details

- **Rendering Engine:** WebGL with custom fragment shaders
- **Effect Algorithm:** Based on complex logarithmic transformations
- **Animation:** RequestAnimationFrame for smooth 60 FPS playback
- **GIF Export:** CCapture.js library for frame capture and encoding
- **Browser Compatibility:** Modern browsers with WebGL support (Chrome 56+, Firefox 52+, Safari 11+, Edge 79+)

## Browser Requirements

- WebGL-enabled browser
- JavaScript enabled
- Minimum 2GB RAM recommended
- Hardware acceleration enabled for best performance

## Troubleshooting

**Image won't load:**
- Check file size (must be under 100MB)
- Verify file format (JPG, PNG, WebP, GIF, or SVG)
- Try a different browser

**Slow performance:**
- Reduce inner levels and outer repeat values
- Lower output dimensions
- Close other applications
- Update graphics drivers

**GIF export fails:**
- Ensure animation speed is not 0
- Try smaller dimensions (512×512 or 1024×1024)
- Check available disk space
- Allow the export to complete (may take 30+ seconds)

**Canvas appears blank:**
- Check if WebGL is enabled in your browser
- Try refreshing the page
- Update your browser to the latest version

## Credits

Created by [Samolevsky.com](https://samolevsky.com)

## License

MIT License - Feel free to use, modify, and distribute this application.

## Support

For issues, questions, or feature requests, please visit [Samolevsky.com](https://samolevsky.com)

---

**Enjoy creating infinite spirals!** 🌀
