# One-Source-Mobility

Landing pages for One Source Mobility accessibility solutions.

## Landing Pages

This repository contains HTML landing pages and their corresponding Gutenberg JSON files for WordPress integration:

### Available Pages

1. **VA Housing Grants** (`va-housing-grants.html`)
   - WordPress slug: `/va-housing-grants`
   - Gutenberg JSON: `va-housing-grants-gutenberg.json`
   - Beaver Builder JSON: `va-housing-grants.json` (legacy)

2. **Commercial Ramps** (`commercial-ramps.html`)
   - WordPress slug: `/commercial-ramps`
   - Gutenberg JSON: `commercial-ramps-gutenberg.json`

3. **Types of Contractors** (`types-of-contractors.html`)
   - WordPress slug: `/types-of-contractors`
   - Gutenberg JSON: `types-of-contractors-gutenberg.json`

4. **Ceiling Track Systems for Schools** (`ceiling-track-systems-for-schools.html`)
   - WordPress slug: `/ceiling-track-systems-schools`
   - Gutenberg JSON: `ceiling-track-systems-for-schools-gutenberg.json`

## Gutenberg JSON Format

The Gutenberg JSON files follow the specification for programmatic WordPress page creation using Gutenberg blocks. Each file includes:

- **title**: Page title
- **status**: Publication status (default: "publish")
- **blocks**: Array of Gutenberg blocks (heading, paragraph, list, image, etc.)

### Supported Block Types

- `core/heading` - Headings (h1-h6)
- `core/paragraph` - Text paragraphs
- `core/list` - Ordered and unordered lists
- `core/image` - Images with captions
- `core/quote` - Blockquotes
- `core/code` - Code blocks
- `core/html` - Custom HTML

## WordPress Integration

The `index.json` file maps WordPress slugs to their source HTML and Gutenberg JSON files for use with the Pull n Press plugin.

Example entry:
```json
{
  "wp_slug": "/commercial-ramps",
  "source_path": "/commercial-ramps.html",
  "gutenberg_json": "/commercial-ramps-gutenberg.json"
}
```