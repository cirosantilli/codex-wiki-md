# Bellman expectation equation

↑ **Parent:** [Bellman equation](bellman-equation.md)

For a finite [Markov decision process](markov-decision-process.md) under fixed policy $\pi$, bounded reward [vector](vector.md) $r^\pi$ and $0\le\gamma<1$, splitting the discounted return at its first step gives $V^\pi=r^\pi+\gamma P^\pi V^\pi$. A [stochastic matrix](stochastic-matrix.md) has supremum-norm operator bound one, so $\sum_{k\ge0}(\gamma P^\pi)^k$ converges and $V^\pi=(I-\gamma P^\pi)^{-1}r^\pi$. This is policy evaluation, not optimization over actions.

**Table of contents**

- [Bellman expectation operator](bellman-expectation-operator.md)

## ↑ Ancestors (6)

1. [Bellman equation](bellman-equation.md)
2. [Dynamic programming](dynamic-programming.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-how-to-build-a-brain-from-scratch-course-of-the-university-of-oxford/2022/4/solution.md)
- [Policy evaluation](policy-evaluation.md)
