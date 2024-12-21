Task-Specific Modular Neural Networks for ARC Benchmark

This repository contains the code and resources for our approach to solving tasks in the Abstraction and Reasoning Corpus (ARC) benchmark using modular neural networks. Our model leverages pixel-based substitutions and encoder-decoder mechanisms to achieve task-specific generalization.

Table of Contents

Project Structure

Installation

Usage

Training

Testing

Visualization

Reproducing Results

Acknowledgments

Project Structure

The repository is organized as follows:

ARC/
|-- configs/                # Configuration files for training
|-- outputs/                # Logs and outputs from experiments
|-- src/                    # Source code for training, testing, and utilities
|   |-- arc/                # Core ARC task processing logic
|   |-- notebooks/          # Jupyter notebooks for EDA and result visualization
|   |-- utils/              # Helper functions for analysis and visualization
|-- README.md               # Project overview (this file)

Key Files
src/train.py: Script for training the model.
src/test.py: Script for testing the trained model.
configs/train.yaml: Configuration for training hyperparameters.
notebooks/: Contains Jupyter notebooks that I used as a reference.

Installation

Clone this repository:

git clone https://github.com/your-username/ARC-with-Neural-Network.git
cd ARC

Install required dependencies:

pip install -r requirements.txt

Usage
Training

Train the model using the following command:

python src/train.py --config configs/train.yaml

Adjust hyperparameters in configs/train.yaml as needed.

Testing

Test the trained model on validation or test datasets:

python src/test.py --config configs/test.yaml

Visualization

Explore results or visualize training logs using the notebooks in src/notebooks/:

look-at-train-data.ipynb: Visualizes the training data.

visualize_test_results.ipynb: Displays predictions and evaluates model performance.

Reproducing Results

To reproduce the results reported in our study:

Use the provided training configuration (configs/train.yaml).

Run the train.py script to train the model.

Use test.py to evaluate the trained model on the test dataset.

Visualize results using the notebooks provided in notebooks/.

Results Summary

Task Accuracy: 44.4%

Pixel Accuracy: 85.7%

Acknowledgments

This project is inspired by the work of Levy et al. and their ARC network architecture. We extend their approach with novel enhancements for task-specific reasoning.

