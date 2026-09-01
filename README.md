# Shard Tools

Privacy-first browser tools for PDFs, images, developer data, text, calculations, documents, and everyday tasks.

**Supported file tools process files locally in your browser without uploads.**

[Visit Shard Tools](https://shard.tools/)

## Why Shard Tools?

Most online file utilities require users to upload personal files to a remote server. Shard Tools takes a local-first approach:

- Files are processed locally for supported tools
- No account is required
- Results are generated directly in the browser
- Tools work on desktop and mobile browsers
- Privacy claims can be independently inspected

## Tools

### PDF

- Merge, split, rotate, and reorder PDF pages
- Delete or extract PDF pages
- Convert PDFs to JPG, PNG, text, or Markdown
- Convert images to PDF
- Compress PDFs to specific file-size targets
- Create, organize, and inspect documents

### Images

- Convert between JPG, PNG, WebP, AVIF, BMP, HEIC, and other formats
- Compress images to specific file-size targets
- Resize images to exact pixel dimensions
- Crop images and create circular crops
- Prepare passport, visa, profile, and application photos
- Create banners and other fixed-size graphics

### Developer and data

- Format, validate, compare, escape, and convert JSON
- Convert between JSON, CSV, XML, and YAML
- Encode and decode Base64, Base32, binary, and hexadecimal data
- Decode JWTs
- Generate UUIDs and hashes
- Format CSS, SQL, and other structured text

### Calculators and generators

- Finance and business calculators
- Construction and measurement calculators
- Unit converters
- Invoice, estimate, quote, and credit-note generators
- Text and data generators

These are representative tools. Browse the complete directory at [shard.tools](https://shard.tools/).

## Privacy

Shard Tools is built around browser-local processing. Supported file tools use browser APIs to decode, transform, encode, preview, and download results without sending the selected file to Shard Tools.

The website may still download application code, fonts, advertisements, directory badges, optional processing models, and other page resources. These requests are separate from transmitting a selected file.

Read the full [privacy policy](https://shard.tools/privacy).

## Privacy proof

The [Shard Tools Privacy Proof](https://shard.tools/privacy-proof) performs a real 200x200 image resize while measuring data-capable browser requests immediately before and after processing.

It distinguishes local file processing from ordinary page downloads and discloses third-party services. Visitors can run the built-in sample or select their own image and independently verify the result using the browser Network panel.

The related [200x200 image resizer](https://shard.tools/tools/resize-image-to-200x200) provides crop-to-fill and fit-with-background modes without stretching the source image.

## Local development

### Requirements

- Node.js 22.13.0 or newer
- npm

### Setup

1. Clone the repository with `git clone https://github.com/Shard-Tools/shard.tools.git`.
2. Enter the project directory with `cd shard.tools`.
3. Install dependencies with `npm install`.
4. Start the development server with `npm run dev`.
5. Open the local address displayed in the terminal.

## Tests and build

- Run the complete test suite with `npm test`.
- Create a production build with `npm run build`.
- Run the linter with `npm run lint`.

## Deployment

The production application is deployed to Cloudflare Workers.

Run `npm run deploy:cloudflare` from an authenticated Cloudflare Wrangler environment with access to the correct account and Worker.

## Project structure

- `app/` - pages, routes, shared interfaces, and tool runners
- `src/engines/` - browser-local processing engines
- `registry/tools/` - tool definitions, metadata, and explanatory content
- `tests/` - unit and rendered-page tests
- `public/` - static assets and locally served runtime files
- `build/` - registry, content, and build-generation scripts
- `docs/` - implementation notes and project documentation

## Contributing

Bug reports and focused improvement suggestions are welcome through [GitHub Issues](https://github.com/Shard-Tools/shard.tools/issues).

Before submitting a code change:

1. Install the project dependencies.
2. Run `npm test`.
3. Run `npm run lint`.
4. Explain the behavior changed and how it was verified.

## Official links

- Website: [shard.tools](https://shard.tools/)
- Privacy proof: [shard.tools/privacy-proof](https://shard.tools/privacy-proof)
- X: [@Shard_Tools](https://x.com/Shard_Tools)
- Email: support@shard.tools

## License

Shard Tools is released under the [MIT License](LICENSE).

Copyright (c) 2026 Roshan Dixit, trading as Shard Tools.
