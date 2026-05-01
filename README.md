# Browser Sound Visualiser

Standalone HTML experiments that use the browser microphone input and Web Audio API to draw full-screen canvas audio visualisers.

## Demos

- `spectrum.html` - linear frequency spectrum bars.
- `spectrum-log.html` - logarithmic frequency spectrum bars.
- `spectrum-log-mirror.html` - mirrored logarithmic spectrum bars.
- `spectrum-log-flame.html` - flame-style logarithmic spectrum visualiser.
- `rain.html` - audio-reactive rain/particle visualiser.

Open any HTML file in a browser and allow microphone access to run the visualiser.

## Microphone access

The demos use `navigator.mediaDevices.getUserMedia({ audio: true })` to request microphone input from the browser. Most pages request access when opened; `spectrum-log-flame.html` waits until the page is clicked before starting audio.

Microphone access is controlled by the browser permission prompt and site settings. To stop capture, close the tab or revoke microphone access from the browser's address-bar permission control.
