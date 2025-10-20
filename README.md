# Handwritten Text OCR

This project detects handwritten text in images using Google Cloud Vision API

## Setup

### 1. Get Google Cloud Credentials

1. Go to [Google Cloud Console](https://console.cloud.google.com/)
2. Create a new project
3. Enable the Vision API
4. Create a service account and download the JSON credentials file
5. Save the file to your Google Drive folder

### 2. Update Credentials Path

In the first cell, update the credentials path to your file location:

```python
os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = "/path/to/your/credentials.json"
```

Example:
```python
os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = "/content/gdrive/MyDrive/G_cloud/your-credentials.json"
```

### 3. Update Image Path

In the execution cell, update the image path to your image:

```python
image_path = "/path/to/your/image.png"
```

Example:
```python
image_path = "/content/gdrive/MyDrive/OCR_Sample_IMG/sample1.png"
```

### 4. Run the Notebook

Run the cells in order. The code will:
- Detect handwritten text from your image
- Display the extracted text
- Show an interactive visualization with bounding boxes
