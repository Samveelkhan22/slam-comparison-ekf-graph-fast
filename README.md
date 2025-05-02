# SLAM Algorithms Comparison: EKF-SLAM, Graph SLAM, and FastSLAM

This repository contains a detailed comparison and implementation of three fundamental SLAM (Simultaneous Localization and Mapping) algorithms:

- **Extended Kalman Filter SLAM (EKF-SLAM)**
- **Graph-Based SLAM**
- **FastSLAM (Rao-Blackwellized Particle Filter)**

The objective is to simulate a mobile robot navigating a 2D environment, observing fixed landmarks, and building a map while estimating its trajectory under each SLAM strategy. Each algorithm is implemented in Python using synthetic data to evaluate its accuracy, scalability, and robustness.

---

## 🧠 Algorithms Overview

### 🔹 EKF-SLAM
Maintains a joint Gaussian over robot pose and landmarks. Suitable for small environments but suffers from linearization errors and quadratic complexity.

### 🔹 Graph SLAM
Builds a constraint graph of poses and landmarks, optimized via nonlinear least squares. Ideal for offline or large-scale mapping with loop closure handling.

### 🔹 FastSLAM
Uses particle filters for robot trajectory and individual EKFs for landmark mapping. Balances accuracy and real-time performance.

---

## 📊 Features Compared

- Accuracy of trajectory and map
- Computational complexity
- Loop closure robustness
- Scalability with number of landmarks
- Real-time applicability

---

## 📈 Visual Outputs

Each algorithm outputs:
- Robot trajectory estimate
- Landmark position estimates
- Comparative graphs showing performance

---

## 🛠️ Requirements

- Python 3.8+
- numpy
- matplotlib
- scipy

---

## 📚 References

- Thrun, S., Burgard, W., & Fox, D. (2005). Probabilistic Robotics. MIT Press.
- Montemerlo, M., Thrun, S., et al. (2002). FastSLAM: A Factored Solution to the SLAM Problem.
- Grisetti, G., Stachniss, C., & Burgard, W. (2010). Graph-Based SLAM.
