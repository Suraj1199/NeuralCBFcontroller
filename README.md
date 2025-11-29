# NeuralCBFcontroller: Safe Autonomous Control with Neural Control Barrier Functions

This project explores the integration of Neural Networks (NNs) with Control Barrier Functions (CBFs) to enable safe and robust control for autonomous systems. By learning complex safety constraints through neural networks, the system can guarantee collision avoidance and adherence to operational limits while pursuing high-level objectives in dynamic environments.

## Features

*   **Neural Control Barrier Functions (NCBFs):** Implements and trains neural networks using PyTorch to approximate Control Barrier Functions, providing a data-driven approach to safety-critical control.
*   **Custom CBF-Infused Loss Function:** Develops a specialized loss function that explicitly incorporates CBF conditions during neural network training, ensuring learned policies inherently satisfy safety guarantees.
*   **Optimization-Based Control (CBF-QP):** Integrates Gurobi Optimizer to solve real-time Quadratic Programs (QPs). These QPs generate control inputs that minimize deviation from a desired (e.g., LQR-derived) control signal while strictly enforcing NCBF-derived safety constraints.
*   **Dynamical System Modeling:** Includes detailed modeling, linearization, and discretization of a vehicle/robot system (e.g., cartpole/unicycle dynamics) to accurately represent real-world physical constraints.
*   **Simulated Environment:** Utilizes the PettingZoo multi-agent reinforcement learning environment (`simple_reach_v3`) to simulate the autonomous system's interaction with obstacles and visualize its safe operation.
*   **Performance & Safety Validation:** Demonstrates the ability of NCBFs to maintain system safety even in the presence of challenging obstacles, showcasing the robustness of the proposed control architecture.

## Technologies Used

*   **Python:** Primary programming language.
*   **PyTorch:** For building and training neural networks.
*   **NumPy:** Essential for numerical computations.
*   **SymPy:** Used for symbolic mathematics, including Jacobian calculations for system linearization.
*   **Matplotlib:** For comprehensive data visualization and plotting of system trajectories, safety margins, and control signals.
*   **GurobiPy:** Python API for the Gurobi Optimizer, used for solving the safety-critical quadratic programs.
*   **Python-Control:** Library for classical control theory, employed for designing Linear Quadratic Regulator (LQR) base controllers.
*   **PettingZoo:** Multi-agent framework for simulating dynamic environments.

## Skills Demonstrated

*   **Robotics & Autonomous Systems:** Design and control of dynamic systems in complex environments.
*   **Control Theory:** Application of advanced control techniques, including LQR and Control Barrier Functions.
*   **Machine Learning:** Neural network architecture design, training, and custom loss function development with PyTorch.
*   **Optimization:** Formulation and solution of Quadratic Programs for real-time control with safety constraints.
*   **Mathematical Modeling:** Symbolic and numerical modeling of system dynamics.
*   **Simulation & Data Analysis:** Development and analysis of simulations to validate theoretical concepts.

---
This `README.md` provides a concise yet comprehensive overview suitable for a project portfolio or CV.