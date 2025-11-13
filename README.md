Stochastic SIRD Epidemic Simulation (CTMC)

This project implements and analyses a stochastic SIRD epidemic model using a Continuous-Time Markov Chain (CTMC) and Gillespie’s algorithm.  
It was completed as part of the **ISC2 – Introduction to Stochastic Modelling** course at Université de Technologie de Compiègne.

The repository contains:
- `notebook.ipynb` – full implementation of simulations, analytics, and plots  
- `project_tasks.md` – list of all project questions and objectives  
- `README.md` – overview and usage instructions

---

## 📌 Project Overview

The epidemic model includes four compartments:

- **S** – Susceptible  
- **I** – Infectious  
- **R** – Recovered  
- **D** – Dead  

Transitions between states follow a CTMC with rates:
- Infection: \( \beta \frac{SI}{N} \)
- Recovery: \( \gamma I \)
- Death: \( \nu I \)

The simulation is performed using **Gillespie’s algorithm**, generating full stochastic trajectories until extinction of infection.

---

## 📊 Main Results (see notebook)

✔ 100 stochastic epidemic trajectories  
✔ Mean and variance of extinction time  
✔ Distribution of infections at half extinction time  
✔ Final epidemic size (mean + variance)  
✔ Plot of S, I, R, D for multiple trajectories  
✔ Estimation of the basic reproduction number \( R_0 \) from early exponential growth  
✔ SEIRD extension including a latent (exposed) compartment  

All results are reproducible directly from the notebook.

---

## ▶️ How to Run

1. Open the notebook: 
```bash
project.ipynb
```

2. Run all cells to reproduce:
- Simulations  
- Plots  
- Analytics  
- \( R_0 \) estimation  

Python libraries required:
- numpty
- pandas
- matplotlib