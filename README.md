# High-Accuracy CAPTCHA Solver with OCR and Image Preprocessing

A Python automation project that uses Selenium, OpenCV, and Tesseract OCR to capture and process a simple image-based CAPTCHA.

## Overview

The script opens a web page with Firefox, locates the CAPTCHA image, captures it, preprocesses the image with OpenCV, and uses Tesseract OCR to extract the CAPTCHA text.

The recognized text is then entered into the target form when the extracted value matches the expected five-character format.

## Features

- Firefox browser automation with Selenium
- CAPTCHA image capture
- OpenCV-based image preprocessing
- Tesseract OCR
- Multiple OCR configurations
- Basic validation of the extracted CAPTCHA text
- Automatic text entry into the target form

## Workflow

1. Start Firefox through Selenium.
2. Open the configured target page.
3. Locate the CAPTCHA image.
4. Save a screenshot of the CAPTCHA.
5. Convert the image to grayscale.
6. Apply Gaussian blur and thresholding.
7. Apply morphological processing.
8. Run Tesseract OCR with two configurations.
9. Validate the extracted text.
10. Enter the result into the web form when five characters are detected.

## Requirements

Python 3.x and the following packages:

```bash
pip install selenium
pip install opencv-python
pip install pytesseract
pip install numpy
Notes

The OCR and preprocessing pipeline in this repository iq
designed around the example CAPTCHA format and may require adjustment for other CAPTCHA implementations.

Use automated browser interaction only on websites and systems where you have permission to do so.

Author

Morteza Roostaie

GitHub: https://github.com/roostaiemorteza

License

MIT License