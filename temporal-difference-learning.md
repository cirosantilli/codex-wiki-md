# Temporal-difference learning

↑ **Parent:** [Reinforcement learning](reinforcement-learning.md)

A value prediction is updated using a reward and a subsequent prediction: $\delta_t=r_{t+1}+\gamma V(s_{t+1})-V(s_t)$. The linear semi-gradient rule is $\Delta w=\alpha\delta_t x(s_t)$ for $V_w(s)=w^{\mathsf T}x(s)$; the target is held fixed for this update. Terminal-state value is zero in an episodic task.[Abstract and sections 2–3; Machine Learning 3, pp. 9–44: successive predictions and temporal credit assignment](learning-to-predict-by-the-methods-of-temporal-differences-by-richard-s-sutton.md)

**Table of contents**

- [Tabular temporal-difference policy evaluation](tabular-temporal-difference-policy-evaluation.md)
- [Reward prediction error](reward-prediction-error.md)

## ↑ Ancestors (8)

1. [Reinforcement learning](reinforcement-learning.md)
2. [Statistical learning](statistical-learning-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-computational-neuroscience-course-of-the-university-of-oxford/2022/6/solution.md)
- [Solution](past-exam-of-the-how-to-build-a-brain-from-scratch-course-of-the-university-of-oxford/2022/4/solution.md)
- [Solution](past-exam-of-the-neuropsychopharmacology-of-higher-cognition-course-of-the-university-of-oxford/2022/4/solution.md)
