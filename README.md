# AI Data Center Microgrid with Battery Storage Peak-Shaving Controller

## 📌 Project Overview
Artificial Intelligence data centers exhibit highly dynamic, high-power consumption profiles—especially during massive parallel LLM training workloads. This project designs and simulates a **Rule-Based Logic Controller** that dispatches a **Battery Energy Storage System (BESS)** to shave peak power demands, ensuring grid/substation stability and reducing peak demand utility charges.

This entire framework is built in **Python**, designed to run completely open-source and cloud-hosted via Google Colab to maintain a zero-local-storage environment footprint.

## 📊 Key Features
* **Dynamic Load Profiling:** Simulates real-world AI data center loads, combining steady-state cooling/compute overhead with stochastic training spikes.
* **Smart Throttling/Dispatch Logic:** Actively flattens substation power demand when load exceeds a predefined safety threshold ($20\text{ MW}$).
* **BESS Constraints Management:** Dynamically models State of Charge (SoC) bounds ($20\% - 100\%$), charging efficiencies, and maximum charge/discharge rates.

## 📂 Repository Structure
```text
├── notebooks/
│   └── peak_shaving_simulation.ipynb   # Main Google Colab Notebook
├── simulation_results.png              # Output visualization graph
└── README.md                           # Documentation Portfolio
