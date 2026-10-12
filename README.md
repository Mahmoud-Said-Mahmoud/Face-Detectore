# Face Detector

A browser app that recognizes faces from the webcam in real time using [face-api.js](https://github.com/justadudewhohacks/face-api.js).

## How it works

1. Loads the SSD MobileNet, face landmark and face recognition models from `/models`.
2. Builds face descriptors from labeled sample photos in `/labels`.
3. Starts the webcam and matches each detected face against the labeled descriptors, drawing a box and name on the video.

## Tech

HTML · CSS · JavaScript · face-api.js · MediaDevices (webcam) API

## Run locally

The models are loaded over HTTP, so serve the folder instead of opening the file directly:

```bash
npx serve .
```

Then open the app and allow camera access.
