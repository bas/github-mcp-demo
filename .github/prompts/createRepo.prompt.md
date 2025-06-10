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
- The implementation must be pixel-perfect and visually indistinguishable from [ui.png](../../docs/design/ui.png). 
- All spacing, alignment, font sizes, colors, border radii, and element sizes must match the design exactly.
- Use HTML, CSS, and JavaScript
- The styling must be done using https://github.com/primer/css
- Use default styles and make sure the start button is a primary button (green)

## Instructions
- Start by sharing a detailed plan before you begin coding
- Before coding, create a table of all design tokens (colors, font sizes, spacing, border radius, etc.) 
  based on [ui.png](../../docs/design/ui.png) and use only these values.
- Follow the requirements and implement the Langton's Ant simulation as specified in both the PRD and this file
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
  - Page layout and styling
- Once complete and verified:
  - Before finalizing, verify:
    - All element sizes and positions match ui.png
    - All fonts, colors, and spacings are identical
    - No extra or missing visual elements
  - After implementation, describe any visual differences between 
    the result and ui.png, and iterate until there are none.
  - Lastly create a gh-pages branch
