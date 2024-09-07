```markdown
# Cub3D

## Overview

**Cub3D** is a 42 project focused on building a basic 3D game engine using raycasting. Inspired by the classic game **Wolfenstein 3D**, the project requires rendering a 3D environment from a 2D map, allowing player movement and interaction within the world.

## Project Goals

- Implement a 3D graphics engine using **raycasting**.
- Render walls and textures based on a 2D map layout.
- Create player movement controls (forward, backward, strafe, rotation).
- Handle collision detection with walls.
- Implement keyboard controls for smooth player navigation.

## Features

- **Raycasting Engine**: The core of the project, simulating 3D graphics in a 2D world.
- **Player Movement**: Controls for walking, turning, and interacting with the environment.
- **Rendering**: Real-time rendering of walls, textures, and sprites.
- **Collision Detection**: Prevents the player from walking through walls.

## How to Run

### Compilation

Use the provided `Makefile` to compile the program:

```bash
make
```

This will generate the `cub3D` executable.

### Running the Game

You can run the game by providing a valid map file:

```bash
./cub3D <map_file.cub>
```

### Example

```bash
./cub3D maps/example.cub
```

## Controls

- `W` / `S` : Move forward / backward
- `A` / `D` : Strafe left / right
- `Left Arrow` / `Right Arrow` : Rotate the player's view
- `ESC` : Exit the game

## Map Format

The map is defined in a `.cub` file, consisting of:
- `1` for walls
- `0` for empty space
- `N`, `S`, `E`, `W` for the player's starting position and direction.

Example of a simple map:

```
111111
100001
1000N1
100001
111111
```

## Resources

- [42 Cub3D subject](https://cdn.intra.42.fr/pdf/pdf/122814/en.subject.pdf)
- [BEST TUTORIAL FOR RAYCASTING, PLEASE USE THIS AND UNDERSTAND IT INSTEAD OF COPY PASTING LODEV CODE](https://pikuma.com/courses/raycasting-engine-tutorial-algorithm-javascript)
```
