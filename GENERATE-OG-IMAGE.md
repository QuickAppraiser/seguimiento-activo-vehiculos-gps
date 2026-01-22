# Generate OG Image PNG

The file `og-image.svg` contains the social media preview image for Open Graph (Facebook, WhatsApp, LinkedIn, Twitter).

## Quick Generation Methods

### Method 1: Online Converter (Easiest)
1. Go to https://cloudconvert.com/svg-to-png
2. Upload `og-image.svg`
3. Set dimensions to 1200x630px
4. Download as `og-image.png`
5. Place in the root directory

### Method 2: Using Inkscape (Desktop)
```bash
inkscape og-image.svg --export-type=png --export-filename=og-image.png --export-width=1200 --export-height=630
```

### Method 3: Using ImageMagick (Command Line)
```bash
magick og-image.svg -resize 1200x630 og-image.png
```

### Method 4: Using Chrome/Edge Browser
1. Open `og-image.svg` in Chrome or Edge
2. Right-click → "Inspect"
3. Click the three dots → "Capture screenshot"
4. Rename to `og-image.png`

### Method 5: Using Node.js (Automated)
```bash
npm install -g svg-to-img
svg-to-img og-image.svg -o og-image.png -w 1200 -h 630
```

## Verify Generated Image

The final `og-image.png` should be:
- Dimensions: 1200x630 pixels
- Format: PNG
- File size: Under 1MB
- Located in root directory

## Testing

Test your OG image using:
- https://www.opengraph.xyz/url/https://gpscarro.com/
- https://developers.facebook.com/tools/debug/
- https://cards-dev.twitter.com/validator

## Current Status

✅ og-image.svg exists and is properly designed
❌ og-image.png needs to be generated

After generating the PNG, all pages will have proper social sharing previews.
