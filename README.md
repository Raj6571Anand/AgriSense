# Enhanced Differential Evolution and Particle Swarm Optimization for IoT Applications (ASDE)

## 📌 Project Overview

Optimization problems in Internet of Things (IoT) environments are often **high-dimensional, multimodal, and dynamic**. Traditional metaheuristic algorithms such as **Particle Swarm Optimization (PSO)** and **Differential Evolution (DE)** perform well individually but suffer from key limitations—PSO converges fast but stagnates, while DE explores well but converges slowly.

This project proposes a **novel hybrid optimization algorithm** called **Adaptive Swarm–Differential Evolution (ASDE)** that intelligently combines the strengths of PSO and DE to deliver **fast, robust, and adaptive optimization** for real-world IoT applications.

---

## 🚀 Key Contributions

- Proposed **ASDE**, a stagnation-aware hybrid PSO–DE algorithm
- Adaptive DE intervention triggered only when PSO stagnates
- Dynamic parameter tuning inspired by **L-SHADE**
- Superior performance on complex benchmark functions
- Practical IoT implementation via **AgriSense** demo system

---

## 🧠 Core Idea (ASDE Algorithm)

- **Default Engine:** Global-best PSO for fast convergence
- **Failure Detection:** Particle-level stagnation monitoring
- **Escape Mechanism:** DE/rand/1 mutation when stagnation is detected
- **Adaptation:** Success-history based tuning of mutation (F) and crossover (CR)

This design ensures:

- Fast exploitation during early stages
- Strong global exploration when trapped in local optima

---

## 📊 Benchmark Evaluation

ASDE was evaluated against baseline PSO and DE using standard optimization benchmarks:

| Function   | Property Tested           | Result                                              |
| ---------- | ------------------------- | --------------------------------------------------- |
| Sphere     | Convergence speed         | PSO fastest, ASDE competitive                       |
| Rosenbrock | Non-convex navigation     | **ASDE outperformed PSO by 11 orders of magnitude** |
| Rastrigin  | Multimodal escape ability | **ASDE avoided premature convergence**              |

---

## 🌱 IoT Application: AgriSense

**AgriSense** is a prototype IoT-based decision support system that demonstrates ASDE in a real-world context.

### Features

- Smart agriculture optimization
- Crop yield maximization
- Optimized NPK, irrigation, and seed density
- AI-recommended sensor placement
- Real-time re-optimization using IoT feedback

### Optimized Outputs

- Projected yield estimation
- Resource allocation plan
- Phase-wise farming schedule
- Sensor layout visualization
- Risk alerts (e.g., drought detection)

---

## 🛠️ Technologies Used

- **Programming Language:** Python
- **Optimization Techniques:** PSO, DE, Hybrid ASDE
- **Simulation Platform:** Google Colab
- **Application Domain:** IoT, Smart Agriculture

---

## 📁 Project Structure

```plaintext
├── algorithms/
│   ├── pso.py
│   ├── de.py
│   └── asde.py
├── benchmarks/
│   ├── sphere.py
│   ├── rosenbrock.py
│   └── rastrigin.py
├── agrisense/
│   ├── app.py
│   └── utils.py
├── results/
│   └── convergence_plots/
├── report/
│   └── Project_Report.pdf
└── README.md
```




---

## 📈 Experimental Setup

- Population Size: 50
- Dimensions: 10
- Iterations: 1000–2000
- PSO: ω = 0.5, c1 = c2 = 1.5
- DE: F = 0.8, CR = 0.9

---

## 👨‍💻 Team Members

- **Mayank Raj**
- **Raj Anand**
- **Wasim Aktar**
- **Raman Tamang**

---

## 👨‍🏫 Supervisor

**Mr. Joy Samadder**  
Assistant Professor  
Department of Information Technology  
Maulana Abul Kalam Azad University of Technology, West Bengal

---

## 📚 References

- Storn, R., & Price, K. _Differential Evolution_, Journal of Global Optimization, 1997
- Singh et al., _QoS Optimization in IoT Smart Agriculture_, IEEE IoT Journal, 2024
- Chandrasekaran, _DE Framework for IoT-MANETs_, 2023

---

## 📌 Conclusion

ASDE successfully bridges the gap between **speed and robustness**, making it highly suitable for **dynamic, large-scale IoT optimization problems** such as smart agriculture, fog computing task scheduling, and wireless sensor network design.

---

⭐ If you find this project useful, consider giving it a star!
