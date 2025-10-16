# Web-based Captcha Solver App

## Overview

This app solves any captcha and displays it on a webpage. It accepts a URL containing an image of the captcha to be solved as input. By default, it will solve and display a sample captcha. 

The app uses the OpenAI Vision API to solve captchas. This API uses trained machine learning models to read and interpret the text in an image.

## Setup

Follow these steps to get the app running on your local machine:

1. Save the HTML file on your computer.
2. Open the HTML file in your web browser.

## Usage

1. Open the web app in your browser.
2. Append `?url=your_image_url_here` to end of the URL in the address bar, where "your_image_url_here" is the URL of the image file of the captcha you want to solve.
3. Press enter to load the new URL.
4. The web app will now display the image of the captcha as well as the solved text.

Eg: If your local HTML file is hosted at `http://localhost:3000/captcha-solver.html`, navigate to `http://localhost:3000/captcha-solver.html?url=https://.../image.png` to solve a specific captcha.

Alternatively, just navigate to `http://localhost:3000/captcha-solver.html` to solve and display the sample captcha.

Please note that the OpenAI API used to solve captchas has certain rate limits - you may need to wait a few seconds between each request to the API.