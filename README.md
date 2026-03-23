# Wave Function Collapse

Interactive Wave Function Collapse visualizer — watch entropy collapse into beautiful tiled patterns step-by-step.

## Features

- **6 tilesets**: Circuit, Pipes, Terrain, Dungeon, Abstract, Celtic Knot
- **Animated generation**: Watch the algorithm find the lowest-entropy cell, collapse it, and propagate constraints in real-time
- **Entropy heatmap**: Toggle to visualize remaining possibilities per cell
- **Wave front glow**: Orange pulse follows the collapse frontier
- **Adjustable speed**: 1–50 steps per frame
- **Grid sizes**: 20×20 to 60×60
- **Step mode**: Advance one collapse at a time
- **PNG export**: Save the generated pattern
- **Auto-retry**: Automatically restarts on contradiction
- **Keyboard shortcuts**: Space (generate), S (step), E (entropy), P (PNG), 1-6 (tilesets), H (help)

## How It Works

Wave Function Collapse is a constraint-based procedural generation algorithm:

1. Every cell starts in **superposition** — all tile types are possible
2. The cell with **lowest entropy** (fewest remaining possibilities) is selected
3. It **collapses** to a single tile (weighted random)
4. **Constraints propagate** to neighbors — incompatible tiles are eliminated
5. Repeat until every cell is determined

## Tech

Single HTML file. Canvas 2D rendering. No dependencies, no build tools.

## License

MIT
