# Causal Reinforcement Learning for Dynamic Pricing: A Case Study

This repository contains a complete, end-to-end case study exploring the intersection of Reinforcement Learning (RL) and Causal Inference. It demonstrates how a seemingly profitable AI agent can learn a flawed strategy and how causal methods can be used to uncover the hidden costs of this strategy.

## About This Repository

This repository contains two distinct Jupyter Notebooks:

### 1. `End-to-End_Causal_RL_Analysis.ipynb`
This is the **main project file**. It's a single Google Colab notebook that contains the entire workflow from start to finish:
* **Cell 1: Setup:** Installs all necessary Python libraries.
* **Cell 2: Model Training:** Defines the market environment and trains a PPO agent from scratch, saving the model file.
* **Cell 3: Causal Analysis:** Loads the trained model and performs the full causal analysis, generating all the tables and visualizations that prove the project's core finding.

➡️ **Start here to replicate the full study.**

### 2. `Economic_Environment_Sandbox.ipynb`
This is a companion notebook designed for **interactive exploration**. It allows users to:
* Play with the parameters of the simulated market (e.g., base price, seasonality, customer loyalty effects).
* Visualize how different factors impact market demand.
* Gain a deeper, intuitive understanding of the "Digital Twin" environment where the agent was trained.

➡️ **Use this notebook if you want to experiment with the market dynamics yourself.**

## Core Finding: The Illusion of Success

Our analysis revealed that the PPO agent, while appearing successful by traditional metrics, had learned a flawed policy based on a spurious correlation with seasonality. A counterfactual simulation proved that this strategy led to a **loss of ~18% in potential profit** over a 10-year period.

## How to Run
1.  Clone this repository.
2.  Open the desired `.ipynb` file in Google Colab or a local Jupyter environment.
3.  Run the cells in order from top to bottom.