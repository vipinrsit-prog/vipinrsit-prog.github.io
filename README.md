# Vipin Kumar

**PhD Research Scholar** · Department of Information Technology  
Babasaheb Bhimrao Ambedkar University, Lucknow, India


Supervisor: [Dr. Amit Kumar Singh](https://scholar.google.com/citations?user=iL39EgsAAAAJ)

**Research areas:** 
. Open RAN & 6G architectures 
· Multi-agent deep reinforcement learning · Constrained optimisation 
· Autonomous UAV systems

---

## About

I work at the intersection of next-generation wireless networks and multi-agent reinforcement learning. My doctoral research designs distributed control systems for autonomous aerial swarms operating on 6G and Open RAN compliant radio infrastructure — networks in which classical scheduling breaks down and standard reinforcement learning fails to respect safety-critical physical constraints.

---

## Research

### Constraint-Aware Multi-Agent Learning for UAV Swarms

The technical contribution at the centre of my doctoral work is a coupling between constrained optimisation and multi-agent reinforcement learning that keeps learned policies feasibility-preserving at runtime. A maximum-entropy formulation of joint power, sub-carrier, and trajectory allocation is solved via Lagrangian duality; the resulting dual multipliers, which encode the activation level of each physical constraint at every step, are then fed as auxiliary state into the centralised critic of a Multi-Agent Deep Deterministic Policy Gradient (MADDPG) network during training. This *dual-into-critic* coupling — to the best of my knowledge, not yet demonstrated on an O-RAN compliant stack — produces policies that are **constraint-aware rather than constraint-blind**.

### Why this matters

Drone swarms are entering operational use in agriculture, disaster response, infrastructure inspection, and emergency communications. Each of these settings requires dozens of UAVs to share limited radio spectrum under sub-ten-millisecond latency budgets while respecting hard constraints on transmit power, interference temperature, and collision distance. The scheduling problem is too fast for centralised optimisation, and off-the-shelf reinforcement learning routinely violates the safety constraints that real deployments must enforce. Bridging that gap is the practical motivation for the work.

### Methods

- **Optimisation:** Maximum-entropy primal–dual solver in PyTorch
- **Learning:** MADDPG with dual-informed centralised critic
- **Co-simulation:** srsRAN (PHY/MAC) + ns-3 (3GPP TR 38.901 and TR 36.777 channels) + AirSim (six-degree-of-freedom dynamics), integrated at one-millisecond timing resolution
- **Evaluation:** Round-robin scheduling, centralised convex, and vanilla MADDPG baselines across swarm sizes of 10, 25, and 50 UAVs

---

## Technical Skills

- **Languages:** Python, C++, MATLAB
- **Frameworks:** PyTorch, CVXPY
- **Wireless simulation:** srsRAN, ns-3
- **Aerial systems simulation:** AirSim
- **Other:** Git, Linux, LaTeX

---

## Doctoral Supervision

This work is conducted under the supervision of **Dr. Amit Kumar Singh**, Assistant Professor at the Department of Information Technology, Babasaheb Bhimrao Ambedkar University, Lucknow.

- Google Scholar: <https://scholar.google.com/citations?user=iL39EgsAAAAJ>
- ORCID: <https://orcid.org/0000-0001-8269-9318>
- Institutional profile: <https://bbau.irins.org/profile/377847>

---

## Contact

**Email:** vipin.rs.it@bbau.ac.in  
**Department of Information Technology**  
Babasaheb Bhimrao Ambedkar University  
Vidya Vihar, Raebareli Road, Lucknow, Uttar Pradesh 226025, India

---

*Last updated: May 2026.*
