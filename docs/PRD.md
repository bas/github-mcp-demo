# Langton's Ant Simulation - Product Requirements Document

## Overview
The Langton's Ant Simulation is a web-based implementation of the classic cellular automaton created by Chris Langton. It demonstrates emergent behavior through simple rules in a grid-based environment.

## Product Goals
- Create an interactive, web-based simulation of Langton's Ant
- Provide real-time visualization of the ant's movement and pattern formation
- Offer intuitive controls for user interaction
- Display comprehensive statistics about the simulation state

## User Interface Requirements

### Grid Display
- Dimensions: 50 x 50 cells
- Cell Size: 10 x 10 pixels
- Styling:
  - Light gray grid lines
  - Distinct border around the entire grid
  - Black/white cells for visited/unvisited states
  - Red square representing the ant

### Control Panel
Location: Below the grid
Components:
1. Start/Stop Button
   - Primary button (green when start, default when stop)
   - Clear visual feedback on click
   - Accessible via keyboard

2. Reset Button
   - Returns simulation to initial state
   - Clears all cell colors
   - Resets statistics

3. Speed Control
   - Slider interface
   - Range: 5-50 steps per second
   - Default: 20 steps/second
   - Clear visual feedback

### Statistics Panel
Location: Right side of grid
Metrics Displayed:
- Ant Position (X, Y coordinates)
- Current Direction (Up/Down/Left/Right)
- Simulation Speed (steps/second)
- Steps Taken (counter)
- Cells Flipped (counter)
- Cells Visited (counter)
- Cells Unvisited (counter)
- Black Cells (counter)
- White Cells (counter)

## Technical Requirements

### Browser Compatibility
- Support for latest versions of:
  - Chrome
  - Firefox
  - Safari
  - Edge

### Responsive Design
- Single-page layout
- Maintains functionality across device sizes
- Grid scales appropriately
- Controls remain accessible on mobile

### Performance
- Smooth animation at all speeds
- Efficient grid updates
- Minimal memory usage
- Real-time statistics updates

### Accessibility
- WCAG 2.1 AA compliance
- Keyboard navigation support
- Screen reader compatibility
- Appropriate ARIA labels
- Color contrast compliance

### Technologies
- HTML5 for structure
- Primer CSS for styling
- Vanilla JavaScript for logic

## Simulation Rules
1. At a white square, turn 90° right, flip the color of the square, move forward one unit
2. At a black square, turn 90° left, flip the color of the square, move forward one unit
3. Continue until stopped by user

## Documentation Requirements
- Clear README.md with:
  - Project overview
  - Installation instructions
  - Usage guide
  - Technical details
  - Browser compatibility information
  - Performance considerations

## Success Criteria
- Smooth operation at 50 steps per second
- Correct implementation of Langton's Ant rules
- Accurate statistics tracking
- Responsive design across devices
- Passing accessibility tests
- Clean, maintainable code structure
