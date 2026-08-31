# Cyberpunk Vending Machine

`FM-2814 · Future Mart` is a browser-based single-page demo of an interactive 3D cyberpunk vending machine. The project is built as one standalone HTML file with Three.js loaded from CDN, combining scene setup, UI, animation, and purchase logic in a minimal static package.


## Features

- Interactive 3D vending machine scene rendered with Three.js and WebGL
- Drag-to-orbit and scroll or pinch zoom camera controls
- Clickable products and slot buttons for item selection
- Simulated payment flow with credit balance and cash insertion
- Per-slot stock tracking with sold-out states
- Holographic display that reacts to welcome, selection, vending, thank-you, low-funds, and sold-out states
- Animated dispensing flow with falling product physics and showcase lighting flash
- Rotating lower showcase carousel with featured products
- Procedural canvas-generated textures, labels, neon signage, and weathering
- Neon lighting, emissive materials, and animated glow effects

## Controls

- Drag to orbit the camera around the machine
- Scroll the mouse wheel to zoom
- Pinch on touch devices to zoom
- Click or tap a product or slot code button to select it
- Click or tap the glowing card pad to complete a purchase
- Click the top-left `+ INSERT ¥500` control to add credit
- Click the bill slot on the payment panel to add credit

## Run Locally

No build step or package install is required.

1. Open `cyberpunk-vending-machine.html` in a modern web browser.
2. Make sure you have an internet connection, because Three.js is loaded from `cdnjs.cloudflare.com`.

## Project Structure

- `cyberpunk-vending-machine.html` contains the markup, styles, Three.js scene setup, state management, and animation loop
- `README.MD` contains project documentation
- `LICENSE` contains the MIT license

## Tech Notes

- The machine body, signage, warning labels, and product art are generated with canvas textures at runtime
- Product interaction is handled with Three.js raycasting against clickable meshes
- Purchasing uses a small in-file state flow for selection, balance checks, vending, restocking, and sold-out handling
- Rendering, lighting, materials, and animation all run directly in the browser through Three.js

## License

This project is licensed under the MIT License. See `LICENSE` for details.
