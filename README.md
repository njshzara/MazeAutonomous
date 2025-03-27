# Maze Autonomous

**Advanced Self-Driving Go-Kart vFinal** is an interactive simulation where a go-kart navigates a dynamically generated maze using reinforcement learning (Q-learning). Developed by Navjit, this project combines AI-driven autonomy with manual control, offering an engaging way to explore machine learning and game development.

## Features

- **Autonomous Navigation**: The go-kart uses Q-learning to learn how to reach the goal while avoiding walls, with a reactive wall repulsion system for smoother driving.
- **Curriculum Learning**: The maze size increases every 250 episodes (from 21x15 to 35x25), challenging the AI to adapt to growing complexity.
- **Manual Control**: Take the wheel with arrow keys (Up: accelerate, Down: brake, Left/Right: turn) to explore the maze yourself.
- **Sensor Visualization**: Five sensors (-60° to 60°) detect walls, with optional visual trails showing their range and hits.
- **Training Persistence**: Save and load the Q-table to retain progress across sessions, stored in browser localStorage.
- **Dynamic UI**: Real-time status updates show episode count, steps, successes, and maze size, with controls to pause, save, or switch modes.

## Usage

1. **Run the Game**:
   - Open `maze.html` in a modern web browser (Chrome, Firefox recommended).
   - Alternatively, visit the live demo on [GitHub Pages](https://njshzara.github.io/MazeAutonomous/maze.html) (if hosted).

2. **Modes**:
   - **Training Mode**: Watch the AI learn by default. Click "Pause Training" to stop, "Resume Training" to continue.
   - **Manual Mode**: Click "Enable Manual Drive" to control the go-kart with arrow keys. Click again to revert to AI.

3. **Controls**:
   - **Save Training**: Stores the Q-table and metadata in localStorage.
   - **Load Training**: Restores previous training progress, including maze size.
   - **Clear Training**: Resets all progress and maze to initial size (21x15).
   - **Show Sensors**: Toggle sensor visualization (checked by default).

4. **Gameplay**:
   - Green square: Starting point.
   - Red square: Goal.
   - The go-kart aims to reach the goal without hitting walls, learning over episodes.

## Requirements

- **Browser**: A modern web browser with JavaScript enabled (e.g., Chrome, Firefox, Edge).
- **Internet** (optional): Only needed if hosting on GitHub Pages or accessing online.
- **Local Storage**: ~5MB free space for saving Q-table data (varies with maze size and training duration).

## Installation

1. **Clone or Download**:
git clone https://github.com/njshzara/MazeAutonomous.git


Or download the ZIP from the GitHub repository.

2. **Open Locally**:
- Navigate to the project folder:
cd MazeAutonomous


- Open `maze.html` in your browser:
start maze.html  # Windows
open maze.html   # macOS
xdg-open maze.html  # Linux


3. **Host Online** (Optional):
- Push to GitHub:
git add maze.html
git commit -m "Initial commit: 3D MazeAutonomous"
git push origin master

- Enable GitHub Pages:
- Go to Settings > Pages on GitHub.
- Set Source to `master`, folder to `/ (root)`, and Save.

## Credits

- **Author**: Navjit
- **Built with**: HTML5, JavaScript, Canvas API
- **AI**: Q-learning algorithm with curriculum learning and wall repulsion enhancements

Enjoy watching the go-kart master the maze—or take control and race it yourself!
Notes
Code Blocks: Added for all commands (git clone, navigation, and Git push steps) to ensure clarity and completeness.
Consistency: Matches your repo at https://github.com/njshzara/MazeAutonomous and the 2D code provided (not the 3D version, as per your latest request).
Instructions: Included platform-specific commands for opening maze.html locally, though users can simply double-click it in most cases.
To add this to your repo:

Create a file named README.md in ~/Desktop/Playground/MazeAutonomous.
Copy-paste the content above into it.
Commit and push from your terminal:
bash

Collapse

Wrap

Copy
git add README.md
git commit -m "Added README for Maze Autonomous"
git push origin master