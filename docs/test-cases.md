# Langton's Ant Simulation Test Cases

This document outlines the test cases for the Langton's Ant simulation at https://bas.github.io/langtons-ant/.

## Functional Test Cases

### 1. Initial State Verification
- **Description**: Verify that the application loads with the correct initial state
- **Steps**:
  1. Navigate to the application URL
  2. Check the grid is visible
  3. Check the ant is positioned at the center of the grid
  4. Check all statistics show correct initial values
  5. Check the simulation is not running
- **Expected Results**:
  - Grid is 50x50 cells
  - Ant is visible at position (25, 25)
  - All cells are white
  - Statistics show correct values: Steps: 0, Direction: Up, etc.
  - Start button is green and says "Start"

### 2. Start/Stop Functionality
- **Description**: Verify that the Start/Stop button correctly controls the simulation
- **Steps**:
  1. Click the Start button
  2. Observe the simulation for a few seconds
  3. Click the Stop button
  4. Observe if the simulation stops
- **Expected Results**:
  - When Start is clicked, the button text changes to "Stop" and loses green color
  - The ant moves and cells change color according to rules
  - Statistics update in real-time
  - When Stop is clicked, the button text changes to "Start" and becomes green again
  - The simulation pauses, and the ant stops moving

### 3. Reset Functionality
- **Description**: Verify that the Reset button resets the simulation
- **Steps**:
  1. Start the simulation and let it run for a few seconds
  2. Click the Reset button
  3. Check the grid and statistics
- **Expected Results**:
  - Grid is cleared (all cells are white)
  - Ant returns to the center position (25, 25)
  - All statistics reset to initial values
  - Simulation stops if it was running

### 4. Speed Control
- **Description**: Verify that the speed slider adjusts the simulation speed
- **Steps**:
  1. Start the simulation
  2. Move the speed slider to different positions
  3. Observe the simulation speed
- **Expected Results**:
  - Speed value updates in real-time
  - Simulation speed changes according to the slider position
  - Speed indicator shows the correct value (between 5-50 steps/sec)

### 5. Ant Movement Rules
- **Description**: Verify that the ant follows Langton's rules correctly
- **Steps**:
  1. Start the simulation and observe the ant's movements
  2. Watch several state transitions
- **Expected Results**:
  - At a white square: ant turns 90° right, flips square to black, moves forward
  - At a black square: ant turns 90° left, flips square to white, moves forward
  - Ant stays within the grid boundaries (wrapping around if necessary)

### 6. Statistics Accuracy
- **Description**: Verify that the statistics panel displays accurate information
- **Steps**:
  1. Reset the simulation
  2. Start the simulation and let it run for a specific number of steps
  3. Check each statistic value
- **Expected Results**:
  - Position coordinates match the ant's actual position
  - Direction matches the ant's actual direction
  - Steps Taken increments correctly
  - Cells Flipped, Visited, Unvisited, Black, and White counts are accurate

## UI Test Cases

### 7. Responsive Layout
- **Description**: Verify the application is responsive across different screen sizes
- **Steps**:
  1. Test the application at various viewport sizes
  2. Check if all UI elements remain accessible and functional
- **Expected Results**:
  - UI adapts to different screen sizes
  - All controls remain accessible
  - Grid and statistics panels remain visible and usable

### 8. Visual Appearance
- **Description**: Verify the visual appearance matches the design
- **Steps**:
  1. Compare the application's appearance with the design
  2. Check colors, spacing, and layout
- **Expected Results**:
  - Grid is centered in its container
  - Statistics panel is aligned to the right with consistent spacing
  - Control panel is below the grid with proper spacing
  - Button styles use Primer CSS classes correctly

## Accessibility Test Cases

### 9. Keyboard Navigation
- **Description**: Verify that the application can be used with keyboard only
- **Steps**:
  1. Navigate through the application using Tab key
  2. Activate buttons using Enter/Space
  3. Adjust slider using arrow keys
- **Expected Results**:
  - All interactive elements can be focused using Tab
  - Buttons can be activated using keyboard
  - Slider can be adjusted using keyboard

### 10. Screen Reader Compatibility
- **Description**: Verify the application works with screen readers
- **Steps**:
  1. Enable a screen reader
  2. Navigate through the application
  3. Interact with controls
- **Expected Results**:
  - All UI elements have appropriate labels
  - Screen reader announces state changes
  - Controls are properly described

## Performance Test Cases

### 11. Long-running Simulation
- **Description**: Verify the application performance during long-running simulations
- **Steps**:
  1. Start the simulation at maximum speed
  2. Let it run for at least 5 minutes
  3. Monitor performance and responsiveness
- **Expected Results**:
  - Animation remains smooth
  - UI remains responsive
  - No memory leaks or performance degradation
  - Statistics continue to update correctly
