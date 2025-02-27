# Audio Visualizer using JavaScript

## Overview
This project is an **Audio Visualizer** that allows users to upload an MP3 file and see a real-time visual representation of the audio. It leverages the **Web Audio API** for processing the audio and the **Canvas API** for rendering the visualizations.

---

## Features
- Upload an MP3 file using an `<input>` element
- Process the audio file using the **Web Audio API**
- Convert MP3 data into an array for analysis
- Visualize audio data dynamically on an HTML `<canvas>`
- Continuously update the visualization in real-time as the audio plays

---

## Project Setup
### 1. Create the necessary files
- **`index.html`** – The main HTML structure
- **`script.js`** – JavaScript logic for audio processing and visualization
- (Optional) **`style.css`** – For additional styling (if needed)

### 2. HTML Structure
The HTML file contains:
- An `<input>` element for users to upload an audio file WEB AUDIO API
- A `<canvas>` element to render the visualization CANVAS API
- Basic styling (inline within the HTML file)

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Audio Visualizer</title>
    <script defer src="script.js"></script>
</head>
<body>
    <input type="file" id="audioFile" accept="audio/mp3">
    <canvas id="visualizer"></canvas>
</body>
</html>
```

---

## Processing Audio Data
### 1. Convert MP3 to Array
- Use the **Web Audio API** to decode the audio file into an array of samples.
- Extract frequency data for visualization.

### 2. Setting Up the Visualization
- The **Canvas API** is used to draw bars or waveforms representing the sound.
- The visualization updates dynamically based on real-time frequency data.

### 3. Running the Visualizer in a Loop
- A continuous animation loop ensures the visualization updates as the audio plays.
- This is achieved using `requestAnimationFrame()`.

---

## Running the Project
1. Open `index.html` in a browser.
2. Select an MP3 file using the upload button.
3. Watch the audio visualization in real-time!

---


