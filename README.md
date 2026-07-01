# Alphia Dev

Alphia Dev is a small static WebGL landing page built around an interactive fluid simulation. It presents a full-screen animated canvas, a centered title and tagline, and a set of social links over a high-contrast visual layer.

## Features

- Full-screen WebGL fluid effect with pointer-based interaction.
- Mouse and touch support for drawing color and motion into the simulation.
- Keyboard shortcuts for pausing the animation and triggering random splats.
- Responsive layout with a mobile-friendly presentation.
- Social links for Telegram, GitHub, Discord, and a project website.

## How It Works

The page is intentionally lightweight:

- `index.html` defines the layout, metadata, social links, and canvas.
- `style.css` handles the fullscreen composition, typography, and button styling.
- `assets/script.js` runs the WebGL simulation and input handling.
- `assets/dat.gui.min.js` is included as a vendor dependency, although the GUI is not enabled in the current UI.

There is no build step and no framework layer. The site runs directly in the browser.

## Controls

- Click and drag on the canvas to create fluid splats.
- Tap and drag on touch devices to interact with the simulation.
- Press `P` to pause or resume the animation.
- Press Space to spawn a burst of random splats.

## Running Locally

Because this is a static site, you can open `index.html` directly in a browser. For the most reliable result, serve the folder through a local web server so that all assets load consistently.

Example options:

- Use VS Code Live Server, if installed.
- Use any simple static server such as Python's built-in HTTP server or a local development server from your preferred tooling.

## Project Structure

- `index.html` - page markup and external asset links.
- `style.css` - layout and visual styling.
- `assets/script.js` - WebGL fluid simulation and interaction logic.
- `assets/dat.gui.min.js` - bundled dat.GUI vendor script.
- `assets/LDR_LLL1_0.png` - texture asset used by the simulation.

## Browser Notes

The effect depends on WebGL support. Some visual enhancements, such as bloom and sunrays, may automatically fall back or disable themselves on devices with limited graphics capabilities.

## Credits

This project includes code and ideas from the WebGL fluid simulation ecosystem and references the AquaInkGL / WishMeLz lineage in the console output. Social links and branding are customized for Alphia Dev.
