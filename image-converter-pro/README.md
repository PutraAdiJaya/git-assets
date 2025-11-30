# Image Converter Pro

A powerful and versatile image converter tool designed to help you easily convert, compress, and optimize images across multiple formats.

## Features

- **Multi-format Support**: Convert between popular image formats including JPG, PNG, GIF, WebP, BMP, and more
- **Batch Processing**: Convert multiple images at once to save time
- **Image Compression**: Reduce file size while maintaining quality
- **Image Resizing**: Scale images to specific dimensions or percentages
- **Quality Control**: Adjust compression quality and settings per format
- **Metadata Handling**: Preserve or remove metadata as needed
- **Fast Processing**: Optimized conversion algorithms for quick results

## Installation

### Prerequisites
- [Node.js](https://nodejs.org/) v14 or higher
- npm or yarn package manager

### Setup

```bash
# Clone the repository
git clone https://github.com/PutraAdiJaya/image-converter-pro.git
cd image-converter-pro

# Install dependencies
npm install

# Start the application
npm start
```

## Usage

### Basic Conversion

```bash
# Convert a single image
image-converter-pro --input image.jpg --output image.png

# Batch convert
image-converter-pro --input ./images --output ./converted --format webp
```

### With Options

```bash
# Convert and resize
image-converter-pro --input image.jpg --output image.webp --width 800 --height 600

# Convert with compression
image-converter-pro --input image.png --output image.jpg --quality 85
```

## Supported Formats

- **Input**: JPG/JPEG, PNG, GIF, BMP, WebP, TIFF, SVG
- **Output**: JPG/JPEG, PNG, GIF, WebP, BMP, TIFF

## Configuration

Create a `config.json` file to set default preferences:

```json
{
  "defaultFormat": "webp",
  "defaultQuality": 80,
  "defaultWidth": 1920,
  "defaultHeight": 1080,
  "preserveMetadata": false,
  "outputDirectory": "./converted"
}
```

## API Reference

### Command Line Options

| Option | Description |
|--------|-------------|
| `--input, -i` | Input file or directory path (required) |
| `--output, -o` | Output file or directory path (required) |
| `--format, -f` | Output image format |
| `--quality, -q` | Compression quality (1-100, default: 80) |
| `--width, -w` | Resize width in pixels |
| `--height, -h` | Resize height in pixels |
| `--preserve-metadata` | Keep image metadata (default: false) |

## Examples

### Convert PNG to WebP

```bash
image-converter-pro --input photo.png --output photo.webp
```

### Batch convert to compressed JPG

```bash
image-converter-pro --input ./photos --output ./compressed --format jpg --quality 75
```

### Resize and convert

```bash
image-converter-pro --input large-image.png --output small-image.jpg --width 400 --height 300
```

## Performance

- Average conversion time: < 1 second per image
- Supports images up to 4GB
- Batch processing optimized for 100+ images

## Troubleshooting

### Issue: "Unsupported format"
- Ensure the input format is in the supported list
- Check file extension is correct

### Issue: "Memory error on large files"
- Try processing one image at a time
- Reduce output dimensions if possible

### Issue: "Low quality output"
- Increase the `--quality` parameter (recommended: 85-95 for JPG)
- Avoid excessive compression on PNG to WebP conversion

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Changelog

### v1.0.0 (Current)
- Initial release
- Multi-format support
- Batch processing
- Image compression and resizing
- Command-line interface

## Support

For issues, questions, or suggestions:
- Open an [issue](https://github.com/yourusername/image-converter-pro/issues)
- Email: support@imageconverterpro.com
- Documentation: [Wiki](https://github.com/yourusername/image-converter-pro/wiki)

## Acknowledgments

- Built with modern image processing libraries
- Thanks to all contributors and users for feedback

---

**Image Converter Pro** - Making image conversion simple and efficient.
