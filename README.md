LET-Spine: Analyzing Cervical Stability
This repository contains the computational tools for the LET (Lyapunov-Entropy-Topology) framework. 
The goal of this system is to quantify cervical spine stability and assess the risk of Adjacent Segment Disease (ASD).

The framework evaluates spinal motion across three primary axes:

Dynamical Instability (λmax): Measures how sensitive the motion is to perturbations.

Informational Complexity (H): Tracks the loss of movement regularity and coordination.

Topological Fragility (T): Analyzes the structural integrity and load distribution of the vertebral segments.

Repository Modules

1. LET_Diagnostic_Framework
This is the core engine of the study. It processes kinematic time-series to map the "Stability Gap", the mathematical distance between healthy physiological movement and pathological states.
2. LET-Monte-Carlo-Simulation
This script runs the analysis 1,000 times using random data variations (bootstrapping). It serves as a statistical audit to prove that the results are robust and not caused by measurement noise.
3. LET-Heuristic-Calibration
A utility to tune the weights (w_1, w_2, w_3) of the Risk Score (J). It ensures scale parity, meaning that instability, entropy, and topology all contribute fairly to the final score without one metric dominating the others due to its numerical range.

Key Empirical Results
Validation using the Branney-Breen clinical dataset (N=63) identified a clear pathological signature:
Global Risk Score (J): Approximately 2417.11 for patients vs. ~1500 for healthy controls.
Stress Riser Ratio (T): 0.383 in flexion, indicating a significant loss of structural integrity at the C6-C7 level.
