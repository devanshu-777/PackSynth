# Molecular Dynamics Simulation: A Guided Jupyter Notebook

## 🚀 Project Overview

This project is a guided, interactive workflow for performing molecular dynamics (MD) simulations, built specifically for a hackathon. The goal is to provide a user-friendly, end-to-end pipeline—from molecular modeling to simulation and analysis—all within a single, reproducible Jupyter Notebook.

By combining powerful open-source tools like RDKit, LAMMPS, and py3Dmol, this project democratizes computational chemistry, allowing users to perform complex simulations with a simple, conversational interface.

### Key Features
* **Conversational Interface:** The notebook guides you through the process with plain English prompts.
* **Automated Modeling:** Generates 3D molecular structures from SMILES strings using RDKit.
* **Full Simulation Pipeline:** Programmatically creates LAMMPS input files and executes a short, complete MD run (minimization → NPT equilibration → production).
* **Automated Analysis:** Performs basic structural analysis (e.g., Radius of Gyration) and generates plots.
* **Interactive 3D Visualization:** Renders the molecular structures and simulation trajectories in an interactive 3D viewer right inside the notebook.
* **Reproducible Environment:** Deployed on [MyBinder.org](https://mybinder.org/) to provide a ready-to-use, cloud-based environment.

## 🏃‍♀️ How to Use

The easiest way to run this project is through MyBinder.org. It requires no installation or setup on your local machine.

1.  Click the "Launch Binder" badge below. This will open the project in a live JupyterLab environment.
    [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/devanshu-777/PackSynth/HEAD?filepath=main_simulation.ipynb)

2.  Once the environment is ready (it may take a few minutes for the first launch), the `main_simulation.ipynb` notebook will open.

3.  Read the cells and run them in order. The notebook will guide you through the entire process, from providing a SMILES string to viewing the simulation results.

## 💻 Local Setup

If you prefer to run the project locally, you will need to set up a `conda` environment.

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/devanshu-777/PackSynth.git
    cd PackSynth
    ```

2.  **Create and Activate the Conda Environment:**
    The `environment.yml` file contains all the necessary dependencies.
    ```bash
    conda env create -f environment.yml
    conda activate md-hackathon-env
    ```

3.  **Launch JupyterLab:**
    ```bash
    jupyter lab
    ```

4.  Open `main_simulation.ipynb` in your browser and run the cells.

## 🛠️ Tech Stack

* **Python:** The core programming language.
* **JupyterLab:** The interactive development environment.
* **RDKit:** Molecular modeling, structure generation, and file I/O.
* **LAMMPS:** The powerful molecular dynamics simulator.
* **MDAnalysis:** For analyzing simulation trajectories.
* **py3Dmol:** For interactive 3D visualization.
* **`mp_api`:** To interface with the Materials Project database.
* **`conda` & MyBinder.org:** For environment management and reproducibility.