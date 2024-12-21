# Google-Image-Downloader

## Description 
This project automates an end-to-end image processing workflow that includes downloading images, converting them to grayscale, resizing, compressing them into a ZIP file, and emailing the processed images.

## Project Overview
The pipeline executes the following tasks:

Download Images: Downloads images from the internet based on the given keyword.
Convert to Grayscale: Converts the downloaded images to grayscale.
Resize Images: Scales images by a specified percentage.
Compress Files: Archives the processed images into a ZIP file.
Send Email: Emails the ZIP file as an attachment to a specified recipient.

## Files in the Project

download.py: Downloads images based on a search keyword.
grayscaleconvert.py: Converts images to grayscale.
scale.py: Resizes images based on a specified percentage.
zip.py: Compresses processed images into a ZIP file.
sendEmail.py: Sends the ZIP file to an email recipient.
pipeline.py: Runs the entire image processing pipeline.
main.py: Simplifies the pipeline with predefined parameters.

## Individual Script Execution
Each step can be executed independently:

Download Images:
 ```bash
python download.py <max_num> <keyword> <output_folder>
 ```
Convert to Grayscale:
 ```bash
python grayscaleconvert.py <input_folder> <output_folder>
 ```
Resize Images:
 ```bash
python scale.py <input_folder> <output_folder> <scale_percent>
 ```
Compress Files:
 ```bash
python zip.py <input_folder> <zip_file_name>
 ```
Send Email:
 ```bash
python sendEmail.py <zip_file_path> <recipient_email>
 ```
## Requirements
Python 3.x
Required Libraries:
icrawler
opencv-python
yagmail

## Install dependencies using:
 ```bash
pip install -r requirements.txt
 ```
Example of Directory Structure
 ```bash
ImageDownloader/
├── files/
│   ├── download.py
│   ├── grayscaleconvert.py
│   ├── scale.py
│   ├── zip.py
│   ├── sendEmail.py
├── pipeline.py
├── main.py
├── requirements.txt
 ```

## License
This project is licensed under the MIT License.
