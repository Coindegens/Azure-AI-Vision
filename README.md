# Azure AI Vision Image Analysis

This project demonstrates the use of Azure AI Vision services to analyze images using Python. It performs various computer vision tasks including image captioning, object detection, and people detection.

## Features

- Image caption generation
- Dense caption analysis
- Object detection with bounding boxes
- People detection with bounding boxes
- Tag generation for image content

## Prerequisites

- Python 3.x
- Azure AI Services account
- Azure subscription

## Required Packages

```bash
pip install azure-ai-vision-imageanalysis==1.0.0b3
pip install python-dotenv
pip install pillow
pip install matplotlib
```

## Configuration

1. Create a `.env` file in the project root
2. Add your Azure AI Services credentials:
```
AI_SERVICE_ENDPOINT=your_endpoint_here
AI_SERVICE_KEY=your_key_here
```

## Usage

Run the script with an image file:
```bash
python image-analysis.py images/street.jpg
```

The script will:
- Generate image captions
- Identify objects and draw bounding boxes
- Detect people and draw bounding boxes
- Save analyzed images as 'objects.jpg' and 'people.jpg'

## Output

The script generates two types of output:
1. Console output with analysis results
2. Annotated images with bounding boxes

## Project Structure

```
image-analysis/
├── images/          # Sample images
├── .env            # Environment variables
└── image-analysis.py # Main script
```

## License

MIT

