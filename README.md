# Boids using Vanilla JavaScript (Weekend Project)

Welcome to the "Boids using Vanilla JavaScript" project! This project implements a simple simulation of boids, which are artificial life forms designed to exhibit flocking behavior, using plain JavaScript and HTML5 Canvas.

![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow)
![HTML5](https://img.shields.io/badge/HTML5-5.0-orange)
![CSS3](https://img.shields.io/badge/CSS3-3.0-blue)

## How the Algorithm Works

The boid algorithm simulates the behavior of a flock of birds or a school of fish. Each boid follows a set of rules that dictate its movement based on the positions and velocities of nearby boids. The core rules are:

1. **Avoidance**: Each boid tries to avoid collisions with other nearby boids.
2. **Alignment**: Each boid aligns its direction with the average direction of its neighbors.
3. **Cohesion**: Each boid moves towards the average position of its neighbors.

Additionally, the boids are constrained by the canvas boundaries, making them turn when approaching the edges.

## Functionality of the Code

### Global Variables

- **SPRITE_RADIUS**: The radius of the boid sprite. (min: 5, max: 20)
- **PROTECTED_RANGE**: The distance within which boids avoid each other. (min: 0, max: 500)
- **VISUAL_RANGE**: The distance within which boids align and center themselves with others. (min: 0, max: 500)
- **MARGIN**: The margin from the canvas edges where boids will start turning. (min: 0, max: 500)
- **MAX_SPEED**: The maximum speed a boid can travel. (min: 0.1, max: 100)
- **MIN_SPEED**: The minimum speed a boid can travel. (min: 0.1, max: 100)
- **AVOID_FACTOR**: The factor by which boids avoid each other. (min: 0, max: 20)
- **TURN_FACTOR**: The factor affecting how much boids turn at the canvas edges. (min: 0, max: 20)
- **MATCHING_FACTOR**: The factor by which boids align their speed with neighbors. (min: 0, max: 20)
- **CENTERING_FACTOR**: The factor by which boids center themselves towards neighbors. (min: 0, max: 20)
- **SET_FPS**: Frames per second for the animation. Zero means unlimited. (min: 0, max: 100)
- **NUMBER_OF_BOIDS**: The total number of boids in the simulation.

### Functions

- **`setInputsFromGlobals`**: Initializes the input values in the HTML form with the current global variable values.
- **`updateGlobalsFromInputs`**: Updates the global variables based on the values entered in the HTML form.
- **`resizeCanvas`**: Adjusts the canvas size when the window is resized.
- **`handle_boids`**: Updates the positions and velocities of boids based on the boid rules.
- **`animate`**: Handles the animation loop, updating the canvas and calling the `handle_boids` function.

### User Controls

- **Reload Button**: Reloads the page to reset the simulation.
- **Pause Button**: Toggles the pause state of the simulation.
- **Input Fields**: Adjust parameters such as sprite radius, protected range, visual range, margin, speeds, and various factors. The number of boids can also be changed.

## Adjustable Values

- **Sprite Radius**: Modify the size of the boid.
- **Protected Range**: Adjust the distance at which boids start avoiding each other.
- **Visual Range**: Change the distance within which boids align and center themselves.
- **Margin**: Set the distance from the canvas edges where boids start turning.
- **Max Speed**: Define the maximum speed for boids.
- **Min Speed**: Define the minimum speed for boids.
- **Avoid Factor**: Control how aggressively boids avoid each other.
- **Turn Factor**: Influence how much boids turn when approaching canvas edges.
- **Matching Factor**: Control how boids align their speed with their neighbors.
- **Centering Factor**: Adjust how much boids center themselves towards their neighbors.
- **Set FPS**: Set the frame rate for the animation.
- **Number of Boids**: Adjust the total number of boids in the simulation.

## Demo

You can view a live demo of this project [here](https://avvienash.github.io/Boids/).

Feel free to experiment with the parameters and observe how the behavior of the boids changes in the simulation. Enjoy exploring the flocking behavior algorithm!
