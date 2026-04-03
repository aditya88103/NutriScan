# MintScan Health

Mobile-first barcode scanner that fetches product data from Open Food Facts and shows a simple health score.

## Features
- Live barcode scanning (camera)
- Manual barcode entry
- Health score with quick breakdown
- Local scan history
- Flashlight toggle (when supported)

## Tech
- Vanilla HTML/CSS/JS
- Quagga (barcode scanning fallback)
- Open Food Facts API

## Getting Started
Camera access requires HTTPS or localhost. Run a local server:

```bash
python -m http.server 5173
```

Then open:

```text
http://localhost:5173
```

## Usage
1. Tap **Scan** to start the camera.
2. Hold steady over the barcode.
3. Use the flashlight button in low light (if supported).
4. History is saved locally on the device.

## Notes
- Flashlight depends on device + browser support.
- This project is client-side only; no user accounts.
- Data comes from Open Food Facts and may be incomplete.

## Roadmap
- Multi-language UI (Hindi + English)
- Better product insights for Indian brands
- Offline-friendly history and caching
