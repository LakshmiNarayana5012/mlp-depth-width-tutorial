# mlp-depth-width-tutorial
# Exploring How Depth and Width Influence Multilayer Perceptron Performance

This repository contains the full code, datasets, figures, and tutorial report for a project investigating how **depth** (number of hidden layers) and **width** (neurons per layer) influence the behaviour and performance of a **Multilayer Perceptron (MLP)**.

The project includes:

- A reproducible Jupyter notebook
- Exported datasets used in the experiments
- Figures demonstrating MLP behaviour
- A full PDF tutorial report
- MIT licensing for reuse

The goal is to provide an accessible, educational walkthrough that helps learners understand how neural network architecture decisions impact accuracy, generalisation, and decision boundary complexity.

---

## Project Overview

This study answers a core question:

> **How do depth and width affect the learning capabilities and generalisation of an MLP?**

We approach this question through two complementary analyses:

###  **Quantitative Evaluation (Digits Dataset)**
- Train MLPs with different depths and widths  
- Compare **training** and **test** accuracy  
- Identify signs of **underfitting** and **overfitting**  
- Plot accuracy vs. architecture to visualise trends  

###  **Decision Boundary Visualisation (Moons Dataset)**
- Train shallow, wide, and deep architectures  
- Visualise learned boundaries in 2D  
- Demonstrate how model capacity affects complexity and smoothness  

These experiments reveal how MLPs behave under architectural changes and show when deeper or wider networks help—or hurt—performance.

---

## 📂 Repository Structure

```
mlp-depth-width-tutorial/
│
├── mlp_depth_vs_width.ipynb          # Main experiment notebook
├── Exploring_Depth_Width_MLP.pdf     # Full tutorial report (PDF)
│
├── data/
│   ├── digits_dataset.csv            # Flattened digits dataset
│   └── moons_dataset.csv             # Synthetic 2D dataset
│
├── figures/
│   ├── depth_plot.png                # Accuracy vs depth
│   ├── width_plot.png                # Accuracy vs width
│   └── moons_plot.png                # Decision boundaries
│
├── src/
│   ├── generate_datasets.py          # Optional dataset recreation
│   ├── train_depth_experiment.py     # Optional script version
│   └── train_width_experiment.py     # Optional script version
│
├── README.md
├── LICENSE
└── requirements.txt
```

---

## 📁 Datasets

### **Digits Dataset**
- 1,797 grayscale images  
- Flattened 8×8 pixel grid (64 features)  
- 10 digit classes (0–9)  
- Ideal for testing MLP architecture sensitivity  

### **Moons Dataset**
- Synthetic 2D dataset  
- Designed for visualisation of nonlinear boundaries  
- Demonstrates how depth/width change boundary shape

Both datasets are included in `/data/` for full reproducibility.

---

## 🚀 How to Run the Project

### 1. Install Dependencies

```bash
pip install -r requirements.txt
```

### 2. Open the Notebook

Run all cells in:

```
mlp_depth_vs_width.ipynb
```

### 3. View Results

You will see:

- Accuracy vs **depth** plot  
- Accuracy vs **width** plot  
- Three decision boundary visualisations  
- Printed train/test accuracy values  


## ♿ Accessibility Features

This project was developed with accessibility in mind:

- Colour-blind-friendly colormaps (`viridis`, `cividis`)
- Alt-text descriptions recommended for all figures
- Clear Markdown hierarchy for screen readers
- Optional transcripts for video explanations
- Avoidance of colour-only encoding in plots (markers + linestyles included)

These steps help ensure the tutorial is useful for a wide range of learners.

---

## 📚 Learning Outcomes

By studying this project, students will learn:

- How depth and width influence MLP capacity  
- Why deeper networks are not always better  
- How width affects overfitting risk  
- How architectural changes alter decision boundaries  
- How to interpret accuracy curves  
- How to combine visual and numerical evidence  

This repository is structured to make experimentation simple and intuitive.

---

## License

This project is released under the **MIT License** (see `LICENSE` for details).  
You are free to reuse, modify, and extend the code with attribution.

---

## Contributions

Contributions, improvements, and extensions are welcome.  
Feel free to fork the repository and explore further architectures or datasets!

---

## Acknowledgements

This work uses:

- **scikit-learn** for MLP and datasets  
- **matplotlib** for visualisation  
- **numpy** for numerical operations  

All code and explanations were written originally for an academic tutorial assignment.

---

##  Contact

If you have questions, suggestions, or want help modifying the project, feel free to open an issue or contact the author.
