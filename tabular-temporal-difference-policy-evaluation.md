# Tabular temporal-difference policy evaluation

↑ **Parent:** [Temporal-difference learning](temporal-difference-learning.md)

A sampled transition updates only the visited value: $V(S_t)\leftarrow V(S_t)+\alpha_t\delta_t$, where $\delta_t=R_{t+1}+\gamma V(S_{t+1})-V(S_t)$. Under the fixed policy, its conditional mean is $(T^\pi V)(s)-V(s)$. Standard tabular convergence requires adequate state visitation and step-size/noise conditions; this mean identity alone does not prove convergence for arbitrary function approximation.

## ↑ Ancestors (9)

1. [Temporal-difference learning](temporal-difference-learning.md)
2. [Reinforcement learning](reinforcement-learning.md)
3. [Statistical learning](statistical-learning-split.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-how-to-build-a-brain-from-scratch-course-of-the-university-of-oxford/2022/4/solution.md)
