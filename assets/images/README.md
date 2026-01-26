# Images Directory

This directory contains images and assets for the EduGrid website.

## Structure

```
images/
├── logos/          # Site logos and branding
├── partners/       # Partner organization logos
├── projects/       # Project images and screenshots
├── team/           # Team member photos
└── blog/           # Blog post images
```

## Adding Images

1. Upload images to the appropriate subdirectory
2. Reference them in Markdown:
   ```markdown
   ![Alt text]({{ '/assets/images/your-image.jpg' | relative_url }})
   ```

## Image Guidelines

- **Format**: Use JPEG for photos, PNG for graphics with transparency
- **Size**: Optimize images before uploading (recommended max width: 1200px)
- **Naming**: Use descriptive, lowercase names with hyphens (e.g., `solar-panel-installation.jpg`)
- **Alt Text**: Always provide descriptive alt text for accessibility

## Placeholder Images

For development, you can use placeholder services:
- https://placeholder.com/
- https://picsum.photos/

Example: `https://picsum.photos/800/600`
