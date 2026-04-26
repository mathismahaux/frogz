# frogz

A Phaser-based platformer game where you control a frog-like character that can charge jumps.

## Level Creation

Levels are created using text files where each character represents a different tile type:

- `P` - Platform (green rectangle)
- `F` - Finish line (white rectangle)
- `.` - Empty space

### Example Level File

```
P..............F
...............
...............
...............
...............
...............
...............
P..............P
```

### How It Works

1. Each line in the text file represents a row of tiles
2. The level is automatically divided into a grid based on the world dimensions
3. Platforms and finish lines are created at the corresponding positions
4. The player starts at the left side and must reach the finish line

### Creating New Levels

1. Create a new `.txt` file in the root directory (e.g., `level2.txt`)
2. Design your level using the characters above
3. Update the `preload` function to load your new level file
4. Update the `create` function to use your level data

The game currently loads `level1.txt` by default.
