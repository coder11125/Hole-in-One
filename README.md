# 2D Mini Golf

A fun, interactive 2D mini-golf game built with React, TypeScript, and HTML5 Canvas. Navigate through various courses, avoid obstacles, and try to get the ball in the hole in as few strokes as possible!

## Features

*   **Physics-Based Gameplay:** Realistic ball movement with friction, velocity, and collision detection.
*   **Dynamic Environments:** 
    *   **Grass:** Standard rolling surface.
    *   **Sand Traps:** High friction, slows the ball down quickly.
    *   **Water Hazards:** Resets the ball to its previous position with a penalty stroke.
*   **Interactive Obstacles:**
    *   **Bouncy Pads:** Propel the ball away at high speeds.
    *   **Boost Panels:** Accelerate the ball in a specific direction.
    *   **Moving Bumpers & Blocks:** Timing-based obstacles that block your path.
    *   **Portals:** Teleport the ball across the map.
*   **Level Progression:** Multiple holes with increasing difficulty and unique layouts.
*   **Sound Effects:** Immersive audio for putting, bouncing, and sinking the ball.
*   **AI Caddy (Optional):** Get AI-generated commentary on your shots using the Gemini API (can be toggled in settings).

## Tech Stack

*   **Frontend Framework:** React 18
*   **Language:** TypeScript
*   **Rendering:** HTML5 `<canvas>` API
*   **Styling:** Tailwind CSS
*   **Build Tool:** Vite

## Getting Started (Local Development)

### Prerequisites
Make sure you have [Node.js](https://nodejs.org/) installed on your machine.

### Installation

1. Clone the repository or extract the downloaded source code.
2. Open your terminal and navigate to the project directory.
3. Install the dependencies:
   ```bash
   npm install
   ```

### Running the Game

Start the local development server:
```bash
npm run dev
```
Open the provided local URL (usually `http://localhost:5173` or `http://localhost:3000`) in your web browser to play.

### Building for Production

To create a production-ready build:
```bash
npm run build
```
The compiled files will be generated in the `dist` directory.

## Controls

*   **Aim & Power:** Click (or touch) anywhere on the screen, drag away from the ball to set the angle and power, and release to putt.
*   The longer the drag line, the more powerful the shot.

## Configuration

You can tweak the game's physics, colors, and features by editing the `src/constants.ts` file. 

**Enabling the AI Caddy:**
The AI Caddy is disabled by default to prevent API rate limit errors. To enable it:
1. Open `constants.ts`.
2. Set `export const ENABLE_AI_CADDY = true;`.
3. Ensure you have a valid Gemini API key configured in your environment variables (e.g., `VITE_GEMINI_API_KEY` in a `.env` file).

## License
SPDX-License-Identifier: Apache-2.0
