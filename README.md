
# PeakFinder-SA

A project demonstrating **finding the peak of a simulated terrain** using **Simulated Annealing (SA)** in Python.  

---

## 🧩 Problem Statement

The challenge was to **efficiently locate the global maximum** of a terrain surface represented by scattered `(x, y, z)` data points. The difficulty lay in the **irregular, sparse, and noisy nature of the data**, which made traditional gradient-based optimization ineffective.  

To solve this, I implemented **Simulated Annealing** with multiple random starting points, adaptive step sizes, and early stopping, ensuring the algorithm could explore different regions without getting stuck in local maxima.

---

## 🛠 Solution Overview

- **Data Input:** Randomly generated terrain points (`x`, `y`, `z`) representing a landscape.  
- **Simulated Annealing:** Explored the surface using probabilistic moves and temperature-based acceptance criteria.  
- **Path Recording:** Stored all explored paths to visualize how the algorithm navigated the terrain.  
- **Visualization:** Used `plotly` to plot 3D terrain and overlay SA search paths for analysis.

The solution successfully located the global peak while providing insight into the search process through visualizations.

---

## 📂 Repository Structure

```

PeakFinder-SA/
│
├── Simulated_Annealing.ipynb
|       └── data generator 
|       └── submission.py           # Implements Model class with SA
|       └── visualize_sa.py         # Visualizes SA search paths
└── README.md               

````

---

## ⚡ How to Run

1. Install zip file

2. Run data generator and fit the model:

3. Visualize the search paths

---

## 📝 Key Takeaways

* **Simulated Annealing** is effective for non-convex, noisy optimization problems where gradients are unreliable.
* Multi-start strategy introduced to help **explore multiple regions** and reduce the risk of local maxima.
* Visualizing the search paths provides **intuition into algorithm behavior** and helps debug optimization issues.

---

## 💡 Challenge Reflection

The most challenging aspect was balancing **exploration and exploitation**: ensuring the algorithm explored the terrain enough to find the global maximum while not wasting time in low-potential regions.
Through careful temperature control, early stopping, and multiple starting points, the SA algorithm became both **efficient and robust**, producing reliable peak estimates even on complex simulated landscapes.

