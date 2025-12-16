# Javascript-GNN

Welcome to the **Javascript-GNN** repository! This project is a powerful, interactive, browser-based Graph Neural Network (GNN) playground, implemented in pure JavaScript and HTML. The demo provides a hands-on environment for learning, visualizing, and experimenting with modern GNNs—directly in your browser.

---

## Table of Contents
- [About the Project](#about-the-project)
- [Features](#features)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Vercel Link](#vercel-link)

---

## About the Project

Javascript-GNN allows you to explore the core ideas of Graph Neural Networks (GNNs), which are powerful neural architectures for learning on graph-structured data (such as molecules, social networks, or knowledge graphs)—all using only your browser with no dependencies or build steps.

You can build networks by:
- Configuring node and feature counts, hidden layer sizes, outputs, and message passing layers
- Editing node features and edge lists interactively
- Customizing targets and hyperparameters
- Live-visualizing the training process, metrics, and graph structure

Everything is designed to be editable, visible, and educational—ideal for learning, teaching, or rapid prototyping.

---

### Built With
- **HTML** for a responsive, modern user interface
- **Vanilla JavaScript** for all GNN logic, model training, and live visualization
- **Canvas API** for dynamic graph rendering—no frameworks or dependencies

---

## Features

- **Full backpropagation through all GNN layers**
    - Parameters are updated across message, update, readout, and output layers for true learning, not just output fitting.

- **Directed or undirected graphs, self-loop option**
    - Toggle whether edges are treated as directed/undirected and whether self-loops are included for aggregation.

- **Edge deduplication and validation**
    - Prevents duplicate or invalid edges, with user-friendly feedback.

- **Configurable hyperparameters**
    - Adjust activation type (ReLU, Leaky ReLU, Tanh, Sigmoid), loss function (MSE, Binary Cross-Entropy), learning rate, network depth/sizes, and training epochs.

- **Interactive graph visualization**
    - Fully dynamic, resizable canvas rendering of your network, showing nodes, edges, and embeddings (“node colors light up as the network trains”).

- **Live training metrics**
    - See the current loss, iteration, and delta loss in real time
    - Live loss chart updates on each epoch

- **Model persistence**
    - Save and load trained model weights to/from file

- **Comprehensive input validation and error highlighting**
    - All user inputs for features, edges, and targets have instant feedback and highlighting for rapid debugging

- **Resource usage limits**
    - Sensible browser-friendly limits on network size and training iterations

- **No dependencies**
    - One HTML file, loads instantly without build tools, npm, or server

---

## Getting Started

### Prerequisites
- Any modern web browser (Chrome, Firefox, Edge, Safari, etc.)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/matthewJamesAbbott/Javascript-GNN.git
   ```
2. Open the `index.html` file in your web browser (double-click or open with your browser of choice).

_No build scripts or server processes required._

---

## Usage

After opening `index.html` in your browser:

1. **Configure your network:**  
   - Set the number of nodes, feature dimensions, hidden/output sizes, and message passing layers.
   - Choose directed/undirected and self-loop options as needed.

2. **Edit node features and edge list:**  
   - Input per-node features in the grid or randomize for a new layout.
   - Edit edges as source,target pairs.

3. **Set training parameters:**  
   - Adjust learning rate, activation, loss, and iterations.

4. **Input your target output vector** for supervised learning tasks.

5. **Train the model:**  
   - Click “Train & Predict” to begin training. Watch live metrics and loss chart update.
   - Stop early with the “Stop” button if needed.
   - Experiment by tweaking graph structure or network parameters.

6. **Visualize and interpret:**  
   - The right panel shows dynamic graph visualization—node colors represent embedding magnitude.
   - Click nodes for feature display (when implemented), or inspect output and metrics.

7. **Save or load models** using the provided buttons for reuse or reproducibility.

---

## Vercel Link

You can try the latest version online without any install:
https://vercel.com/msquigs-projects/javascript-gnn-tczb
