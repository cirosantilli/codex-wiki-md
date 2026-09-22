# Verification by a nonnegative control supermartingale

↑ **Parent:** [Hamilton-Jacobi-Bellman equation](hamilton-jacobi-bellman-equation.md)

For a nonnegative classical solution $V$ of a finite-horizon [Hamilton-Jacobi-Bellman equation](hamilton-jacobi-bellman-equation.md) with nonnegative running reward $r$, the process $V(X_t,t)+\int_0^t r(X_s,a_s)ds$ is a local [supermartingale](supermartingale.md) under every admissible control. The [Itô formula](ito-s-lemma.md) gives nonpositive drift because the chosen control cannot exceed the supremum in the equation. Stop where the [stochastic integral](stochastic-integral.md) becomes a true [martingale](martingale-split.md), take expectations and apply the [Fatou lemma](fatou-s-lemma.md). Nonnegativity prevents loss of a lower bound when removing the stops, giving the verification upper bound. A maximizing control attains the bound when its stopped reward processes are [uniformly integrable](uniform-integrability.md).

## ↑ Ancestors (7)

1. [Hamilton-Jacobi-Bellman equation](hamilton-jacobi-bellman-equation.md)
2. [Bellman equation](bellman-equation.md)
3. [Dynamic programming](dynamic-programming.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-42/2/solution.md)
