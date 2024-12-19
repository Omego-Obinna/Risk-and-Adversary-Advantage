# Monte Carlo Simulations for Adversary's Advantage and Risk Assessment 📚💻

## Overview
This repository contains MATLAB simulation codes designed to evaluate the adversary’s advantage $(\mathsf{Adv})$ and associated risk $(R)$ in strategic scenarios between an adversary $(\mathcal{A})$ and a user $(\mathcal{U})$. The simulations explore:

- **Positive Advantage Scenario:** $\mathsf{Adv} > 0$ indicating increased risk to the user.
- **Negative Advantage Scenario:** $\mathsf{Adv} < 0$ indicating reduced or even negative risk to the user.

These Monte Carlo simulations generate results that can be visualized in 3D scatter plots and histograms, providing valuable insights into how changes in parameters influence $(\mathsf{Adv})$ and $(R)$.

---

## Description 📝

**What the Code Does:**
- Implements Monte Carlo simulations by sampling key parameters from specified probability distributions.
- Calculates the adversary’s advantage and risk based on sampled parameters.
- Produces 3D visualizations of the relationships between the probability of attacking $( p^* )$, the probability of hiding $( q^* )$, and the resulting risk.
- Outputs statistical summaries (mean, min, max) of $(\mathsf{Adv})$ and $(R)$.

**Scenarios:**
1. **Positive Advantage:** 
   - Higher benefit for the adversary under certain conditions.
   - Visualizes how user risk can escalate.

2. **Negative Advantage:**
   - Configurations where adversary’s success probabilities are lower when the user hides.
   - Demonstrates how the user might achieve scenarios where the risk is minimized or even negative.

---

## Features 🌟

- **Parameter Sampling:** Randomly sample from uniform and Beta distributions.
- **Probability Constraints:** Ensure $( p^* )$ and $( q^* )$ remain within [0,1].
- **Dynamic Impact Factors:** Compute risk using flexible cost-benefit parameters.
- **Visual Outputs:** Interactive 3D plots and histograms for deeper analysis.
- **Statistical Summaries:** Mean, minimum, and maximum values for both $(\mathsf{Adv})$ and $(R)$.

---

## Files Included 📂

**1. `positive_advantage_simulation.m`**
   - Runs the positive advantage scenario.
   - Generates a 3D scatter plot, histogram, and prints statistical outcomes.

**2. `negative_advantage_simulation.m`**
   - Executes the negative (and zero) advantage scenario.
   - Provides 3D visualization and statistical analysis, including negative risk outcomes.

**3. `simulation_code.zip`**
   - A compressed file containing both simulation scripts and any supporting files for easy distribution and reproduction.

---

## Getting Started 🚀

### Requirements
- MATLAB (R2020a or newer recommended).

### Steps to Run
1. **Setup:** Download or clone this repository.
2. **Unzip Files:** Extract `simulation_code.zip` into your MATLAB working directory.
3. **Open MATLAB:** Navigate to the directory containing the scripts.
4. **Run:** Execute `positive_advantage_simulation.m` or `negative_advantage_simulation.m` from the MATLAB command window or editor.
5. **View Results:** 
   - Examine the 3D scatter plots and histograms in MATLAB figure windows.
   - Review the printed statistics in the command window.

### Customization 🔧
- Modify parameter ranges (e.g., `B_A_leak_range`, `C_U_hide_range`).
- Adjust Beta distribution parameters (`a_beta`, `b_beta`) to shape the hiding effectiveness.
- Experiment with different seeds (`rng()` commands) for reproducibility or variability.

---

## Outputs and Visualization 🖼️

- **3D Scatter Plots:** Display relationships between  $p^* $,  $q^*$, and  $R$ color-coded by $\mathsf{Adv}$.
- **Histograms:** Present distributions of $\mathsf{Adv}$ values, revealing underlying patterns in adversary-user dynamics.
- **Statistics:** Summaries for mean, min, and max values of $\mathsf{Adv}$ and $R$ printed directly to the command window.

---

## Citation and References 📜
If you use these codes in your research, please cite the associated research paper:
> Steganography and Probabilistic Risk Analysis: A Game Theoretical Framework for Quantifying Adversary Advantage and Impact  

---

## License ⚖️
This project is licensed under the Apache-2.0 License. See the `LICENSE` file for details.

---

## Contact 💬
For inquiries, please contact:  
Dr Obinna Omego  
a.omego@kingston.ac.uk, omegoobinna@gmail.com

I hope these simulations assist in exploring various strategic scenarios and enhance the reproducibility of your research!
