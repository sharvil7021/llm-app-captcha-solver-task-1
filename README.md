# Captcha Solver

## Overview
This is a simple web app that can display an image from a specified URL (using the `?url=` query parameter) and attempt to solve the image as a captcha using an OCR (Optical Character Recognition) model from Google's Vision API.

## Setup
To use this app, you will need to replace `<YOUR_API_KEY>` with your actual Google Cloud API Key in the `visionAPI` variable of the `index.html`.

## Usage
Begin by launching the `index.html` file in your web browser.

The app will display the image from the URL specified in the `?url=` query parameter. If no URL is specified, it will display a default 'sample.png' image.

The app will then make a request to the Google Vision API, attempting to interpret any text found in the image. The interpreted text will then be displayed on the screen.

Please note that there is a short delay (around 100 milliseconds) before the app will attempt to solve the captcha. This is to ensure that the image has fully loaded before the Vision API is called. The interpretation should typically take less than 15 seconds, allowing the user to see the solution quite quickly.