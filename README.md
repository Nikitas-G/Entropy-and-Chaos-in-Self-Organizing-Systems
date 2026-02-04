LET-Spine: Computational Framework for Cervical Regime Analysis
This repository provides the implementation of the Lyapunov-Entropy-Topology (LET) framework, 
a multi-objective diagnostic suite for quantifying spinal stability and Adjacent Segment Disease (ASD) risk.

Framework Overview
The LET framework maps kinematic trajectories into a three-dimensional diagnostic manifold to identify transitions between physiological and pathological regimes. 
Core Indicators
Dynamical Instability (λmax): Local stability assessment via the Largest Lyapunov Exponent.
Informational Complexity (H): Quantification of regularity loss through Shannon Entropy.
Topological Fragility (T): Structural integrity analysis via the Stress Riser Ratio and algebraic connectivity.

Repository Architecture
The suite consists of two primary computational modules:

LET_Diagnostic_Framework
Executes state-space reconstruction using time-delay embedding.
Projects the Dynamic Integrity State Vector M(t) onto the diagnostic landscape.
Identifies the "Stability Gap" between the physiological attractor and pathological states.

LET Clinical Validation Report
Performs Monte Carlo bootstrapping (n=1,000) for statistical robustness.
Calculates the Global Risk Score (J) with associated confidence intervals.
Validates the PSO-based navigability of the diagnostic landscape.

LET-Spine: Lyapunov-Entropy-Topology Framework for Cervical Stability Analysis
Implementation of the LET (Lyapunov-Entropy-Topology) diagnostic suite for quantifying self-organization and structural integrity in cervical spine kinematics. This framework maps nonlinear dynamical stability (λmax), informational complexity (H), and spectral graph connectivity (T) onto a unified manifold to identify pathological regime shifts and Adjacent Segment Disease (ASD) risk factors.

Key Empirical Results
Validation using the Branney-Breen dataset identified a distinct pathological signature:
Global Risk Score (J): 2351.55±4.89.
Pathological Stress Riser Ratio: 0.383, indicating significant topological stiffening.
Regime Shift: Observed drift toward λmax≈ 0.56 and decreased entropy (H≈2.65).

Implementation
The scripts are optimized for high-dimensional kinematic time-series analysis.
Input: Multi-segmental translation and angular data.
Output: Comprehensive clinical diagnostic reports and 3D manifold visualizations.
