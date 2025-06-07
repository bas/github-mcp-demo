# Langton's Ant Simulation

Langton's Ant is a two-dimensional Turing machine with a very simple set of rules but complex emergent behavior. In a grid of cells (initially all white), an "ant" moves according to the following rules:

1. At a white square, turn 90° right, flip the color of the square, move forward one unit
2. At a black square, turn 90° left, flip the color of the square, move forward one unit

Despite its simple rule set, the ant's path eventually develops a recurring "highway" pattern of repeating movements.

## Running the demo

The demo runs a sequence of MCP Tool calls that create a repository in your personal account.

1. Install [GitHub MCP Server](https://github.com/github/github-mcp-server#installation).
2. Start the server (requires Docker).
3. Open Copilot Chat in Agent mode (Sonnet models give the best results).
4. Run: `/createRepo`
5. Run: `Add an issue to split HTML, CSS and JS in separate files and assign it to me`
```
Add an issue to split HTML, CSS and JS in separate files and assign it to me
```
6. Run:
```
Fix issue #1 on a separate branch and open a PR
```
7. Check the repository created, the issue, the pull request and the Pages site.

## Acknowledgments

- Chris Langton for creating the original cellular automaton
- The cellular automaton and complexity theory communities
