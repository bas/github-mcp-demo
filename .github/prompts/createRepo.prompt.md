---
mode: 'agent'
description: 'Generate a Langtons Ant simulation.'
tools: ['get_me','create_repository','get_file_contents',
  'create_or_update_file','create_pull_request', 'create_branch', 
  'create_issue', 'update_pull_request_branch']
---
# Langton's Ant Simulation

Create a langton's ant simulation. 

For detailed specifications, please refer to the [Product Requirements Document](../../docs/PRD.md).

## Implementation Requirements
- Create the repository in my personal account
- All code in a single index.html file
- Follow the design provided in [ui.png](../../docs/design/ui.png)
- Use HTML, CSS, and JavaScript
- The styling must be done using https://github.com/primer/css
- Use default styles and make sure the start button is a primary button (green)

## Instructions
- Start by sharing a detailed plan before you begin coding
- Follow the requirements and implement the Langton's Ant simulation as specified in both the PRD and this file
- Pay special attention to matching the UI design exactly:
  - Grid must be centered in its container
  - Statistics panel must be aligned to the right with consistent spacing
  - Control panel must be below the grid with proper spacing between buttons and slider
  - Font styles, sizes, and colors must match the design
  - Button styles must use Primer CSS classes correctly
  - Spacing between elements must match the design exactly
- During implementation, continuously verify against:
  - The PRD requirements
  - The UI design in ui.png
  - The technical specifications
- Test the implementation thoroughly, especially:
  - The ant's movement rules
  - Statistics accuracy
  - Performance at different speeds
  - Responsive behavior
  - Accessibility features
- Once complete and verified:
  - Create a gh-pages branch
  - Verify the deployment works correctly
