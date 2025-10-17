# Captcha Solver

## Overview

The Captcha Solver is a single-page web app designed to solve captchas using an external API. The app fetches an image from a provided URL (via a `?url=` query parameter), or defaults to an attached sample image, and solves the captcha within 15 seconds. The solution, as well as the image itself, are then displayed on the page. 

## Setup

To setup the Captcha Solver web app on your local machine, use the following steps:

1. Download `index.html` to your preferred location on your local machine.
2. Open `index.html` file in any web browser of your choice.

## Usage

To use this captcha solver, you need to provide a URL of an image by appending `?url=<your-image-url>` to the end of the page's URL in the address bar. If no URL parameter is provided, the app will default to solving the attached sample image.

Please note, as this is a demo version, the backend API (`https://api.example.com/data`) is a placeholder. In a production setting, you would replace this with the endpoint of an OCR service, like the OpenAI Vision API.

## Improvements

As this is version 1.0 of the Captcha Solver, no improvements from a previous version can be listed yet.