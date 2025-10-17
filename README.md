## Captcha Solver App

This is a simple, lightweight web app designed to test the functionality of an OCR (Optical Character Recognition) captcha solving service.

### Usage

Run the app and it will automatically start attempting to solve a captcha whose URL has been provided in the "url" query parameter. If no URL is provided, it will attempt to solve a default image whose data is stored in the source code as a Base64 string.

Please be aware that the app runs 100% client-side (there is no server component). Consequently, the app will attempt to make a POST request to a local endpoint (`/api/solve-captcha`) with the Base64 data as the payload, where it is expected that the captcha will be solved. However, unless you have an appropriate service running at that endpoint, you will simply receive an error.

You can customize this endpoint by modifying the `SOLVER_API_ENDPOINT` constant in the source code.