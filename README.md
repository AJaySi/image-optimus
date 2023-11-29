# Image Compression and Conversion Tool

A versatile Python tool for effective image compression and conversion. It includes local compression options, WebP format conversion, and integration with the Tinyfy API for advanced image compression.

## Features

- **Local Image Compression**: Compress images with adjustable quality and the option to resize.
- **WebP Conversion**: Efficiently convert images to the WebP format for optimized web usage.
- **Tinyfy API Integration**: Harness the power of the Tinyfy API for superior image compression.
- **Batch Processing**: Perform operations on entire directories, processing numerous images at once.
- **EXIF Data Preservation**: Preserve EXIF data during compression for images where metadata is crucial.
- **Verbose Logging**: Detailed logging for enhanced tracking and debugging of the compression and conversion processes.

## Installation

To get started, ensure Python is installed on your system. The tool relies on several Python libraries including Pillow, loguru, tqdm, and tinify, which can be installed using pip:

```bash
pip install Pillow loguru tqdm tinify
```
Note: You'll need an API key from Tinyfy for the Tinyfy API integration. Set this key as an environment variable TINIFY_API_KEY.

## Usage

### Compress Images Locally

Compress all images within a specified directory, adjusting quality, size, and EXIF data preservation as needed:

```python
compress_images_in_directory('/path/to/your/images', quality=85, resize=(800, 600), preserve_exif=True)
```
### Compress Images Using Tinyfy API

Utilize the Tinyfy API for advanced compression on images within a directory:
```python
compress_images_in_directory_tinyfy('/path/to/your/images')
```
### Convert Images to WebP

Convert all images in a directory to the WebP format:
```python
convert_directory_to_webp('/path/to/your/images')
```
