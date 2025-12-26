# Amazon Title Optimizer

A client-side tool for bulk Amazon listing title optimization. No backend, no API keys, no accounts required.

**Built for CEYBO remote control inventory management.**

## Quick Start

1. Open `index.html` in your browser (or visit the deployed GitHub Pages URL)
2. Click **"Download Template"** to get a blank CSV with correct headers
3. Upload your inventory file (CSV or Excel)
4. Map your columns to the required fields
5. Click **"View Examples"** to see what each strategy generates
6. Select your optimization strategy
7. Click **"Generate Titles"**
8. Use **"Mobile View"** toggle to see 150-char mobile cutoff
9. Click 📋 to copy individual titles
10. Download the optimized file
11. Upload to Amazon Seller Central via bulk edit

## Features

### Optimization Strategies (v1.1 - Part# Front-Loaded)

| Strategy | Best For | Title Format |
|----------|----------|--------------|
| **OEM Premium** | Authorized resellers | `BN59-01178B Original OEM Remote Control for Samsung UN55F6300 TV - Genuine Replacement` |
| **Compatible Mid-Range** | Third-party products | `BN59-01178B Compatible Remote Control for Samsung UN55F6300 TV - Universal Replacement` |
| **Universal Budget** | Generic products | `Universal Remote Control for Samsung UN55F6300 TV - Works with BN59-01178B` |

**Key v1.1 Change:** Part numbers are now front-loaded in OEM and Compatible strategies because customers search by part number when their remote breaks.

### Options

- **Spanish Keywords**: Appends bilingual terms (e.g., `| Control Remoto Original`)
- **Mobile-First**: Shows 150-char cutoff indicator in preview
- **Subject Matter Fields**: Generates 5 CEYBO-specific indexing keywords:
  1. `[Brand] TV Remote Control`
  2. `[Part Number] Replacement Remote`
  3. `Universal Remote for [Brand] [Model]`
  4. `OEM [Brand] Remote Parts`
  5. `Smart TV Remote Control Accessories`

### New in v1.1

- ✅ **Part# front-loaded** in OEM and Compatible strategies
- ✅ **"View Examples" button** - see title output before processing
- ✅ **"Download Template" button** - blank CSV with correct headers
- ✅ **Copy to Clipboard** - click 📋 on any title row
- ✅ **Mobile View toggle** - shows 150-char cutoff with visual indicator
- ✅ **Live character count** - color-coded (green/yellow/red)

## File Requirements

### Input Columns

| Column | Required | Description |
|--------|----------|-------------|
| SKU | ✅ | Your seller SKU |
| Part Number | ✅ | Manufacturer part number |
| Brand | ✅ | Brand name |
| Model | ❌ | Model number/name |
| Current Title | ❌ | Existing title (for reference) |
| Price Tier | ❌ | Premium/Mid-Range/Budget |

**Note:** Column names are flexible. The tool will auto-detect common variations.

### Output Columns

Your original file plus:
- `Optimized Title` - The generated title
- `Char Count` - Character count
- `Status` - ✅ (good), ⚠️ (warning), ❌ (error)
- `Warnings` - Any issues detected
- `Subject Matter 1-5` - If enabled

## Validation Rules

- **Maximum length**: 200 characters (Amazon limit)
- **Minimum length**: 60 characters (recommendation)
- **Special characters**: Flagged for review

## Privacy

**Your data never leaves your browser.** All processing happens client-side. No servers, no tracking, no data storage.

## Supported File Formats

- CSV (.csv)
- Excel (.xlsx, .xls)

Output format matches input format.

## Browser Support

Works in all modern browsers:
- Chrome (recommended)
- Firefox
- Safari
- Edge

## Deployment

To deploy on GitHub Pages:

1. Create a new repository
2. Upload all files
3. Go to Settings → Pages
4. Select "Deploy from a branch" → main → / (root)
5. Your tool will be live at `https://[username].github.io/[repo-name]/`

## Troubleshooting

**File not loading?**
- Check file format (CSV or Excel only)
- Ensure file has column headers
- Try re-saving from Excel as .xlsx

**Columns not detected?**
- Use standard column names (SKU, Part Number, Brand, Model)
- The mapping modal lets you manually assign columns

**Characters showing incorrectly?**
- Ensure your file is saved with UTF-8 encoding

## Version

v1.1 - Part# front-loading, View Examples, Download Template, Copy buttons, Mobile View

---

Built for Jared @ CEYBO. Questions? You know where to find me.
