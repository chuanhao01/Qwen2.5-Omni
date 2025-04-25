# Running the web_demo locally with https

This is because when running it locally on http, security settings on browsers prevents access to the webcam and microphone.
As such this fork and branch fixes this.

## Setup

1. Create self signed certificate for SSL
   1. `openssl req -newkey rsa:2048 -new -nodes -x509 -keyout key.pem -out cert.pem`
2. Install requirements
   1. `python -m venv .venv`
   2. `source ./.venv/bin/activate`
   3. `pip install -r requirements_web_demo.txt`
