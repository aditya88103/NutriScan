# NutriScan

NutriScan is a mobile-first barcode scanner that pulls product data from Open Food Facts and shows a simple nutrition score (0–10).

## Features
- Fast live scanning (BarcodeDetector when available, with Quagga fallback)
- Flashlight toggle (when supported by device/browser)
- Manual barcode entry
- Nutrition score with quick breakdown
- Product details + nutrition table + ingredients/allergen highlights (only shows available fields)
- Local scan history (stored on-device, no account)

## Data Source
NutriScan uses Open Food Facts (community-powered). Coverage varies, so some Indian products may be missing or incomplete.

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
- Offline-friendly history + caching
