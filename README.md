# aisc-project
Project Description

A* 3D Visualizer is an interactive web application designed to make graph pathfinding algorithms intuitive and easy to explore. It automatically generates a 3D force-directed layout for custom graph structures and animates the step-by-step execution of the A* search algorithm in real-time. Users can define custom nodes, heuristic values, edge costs, start nodes, and goal nodes while inspecting open and closed lists, path costs, and heuristic admissibility.

Features

3D Force-Directed Layout: Positions graph nodes in 3D space using a spring-embedder simulation algorithm.

Interactive Viewport: Rotate, pan, and zoom using standard mouse controls or toggle automatic scene rotation.

Custom Graph Builder: Easily input custom graph nodes with heuristics and weighted undirected edges.

Execution Modes: Step through algorithm iterations manually or set automatic execution with adjustable speed controls.

Admissibility Warning: Detects whether the specified heuristic values overestimate remaining path costs.

Live State Logging: Displays live contents of the sorted Open list (with g, h, and f values), Closed list, step log, and calculated shortest path.

Tech Stack

Frontend: HTML5, CSS3, JavaScript (ES6+)

3D Engine: Three.js (r128)

Getting Started

No build tools or external dependencies installation are required.

Clone or download the repository:

git clone https://github.com/your-username/Astra-3d.git
cd Astra-3d


Open index.html in your preferred web browser, or launch it using a local development server (such as Live Server in VS Code).

How to Use

Nodes: Enter nodes one per line using NodeName HeuristicValue (e.g., S 7).

Edges: Enter undirected edges one per line using FromNode ToNode Cost (e.g., S A 1).

Start & Goal: Define the starting node and target goal node.

Build Graph: Click Build graph to generate the node positions and edges in 3D space.

Run Algorithm: Click Run to start the search or Step to advance one iteration at a time.

Project Structure

Astra-3d/
├── index.html    # Application structure and control panel
├── style.css     # UI styling and light/dark theme rules
└── script.js     # Three.js 3D rendering and A* algorithm engine
