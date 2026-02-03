# AI Tag Generator

A simple tool to automatically generate tags for images using Artificial Intelligence (wd-swinv2-tagger-v3).
Ideal for organizing image datasets for LoRAs training, Stable Diffusion, or simply for cataloging.

## Features

**Automatic Detection**: Identify content and characters in images.
**Batch Processing**: Process hundreds of images at once.
**Intelligent**: Skips files that have already been processed to save time.
**Resilient**: Continues the process even if an image fails.
**Reports**: Displays success and failure statistics at the end.

## How to use

### 1. Prerequisites

Make sure you have Python installed. Install the dependencies by running:

```bash
pip install -r requirements.txt
```

### 2. Preparation

1. Create a folder called `imgs` in the same location as the script.
2. Place all your images (`.jpg`, `.png`, etc.) inside it.

### 3. Execution

Open the terminal and run:

```bash
python tag_generator.py
```

The script will:
1. Connect to the AI API.
2. Read the images from the `imgs` folder.
3. Save the text files (`.txt`) with the tags in the `txts` folder.

## Advanced Settings

You can change some settings directly in the `tag_generator.py` file:

- **TEMPLATE**: Change the tagger template if desired.
- **THRESHOLDS**: Adjust the sensitivity of tag detection.

## Credits

Use the [SmilingWolf/wd-swinv2-tagger-v3](https://huggingface.co/SmilingWolf/wd-swinv2-tagger-v3) template via Gradio Client.
