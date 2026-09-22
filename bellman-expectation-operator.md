# Bellman expectation operator

↑ **Parent:** [Bellman expectation equation](bellman-expectation-equation.md)

The operator $T^\pi V=r^\pi+\gamma P^\pi V$ performs one exact fixed-policy backup. Since each row of $P^\pi$ averages component differences, $\|T^\pi V-T^\pi U\|_\infty\le\gamma\|V-U\|_\infty$. The [Banach fixed-point theorem](contraction-mapping-theorem.md) then gives a unique bounded [fixed point](fixed-point.md) for $0\le\gamma<1$.

## ↑ Ancestors (7)

1. [Bellman expectation equation](bellman-expectation-equation.md)
2. [Bellman equation](bellman-equation.md)
3. [Dynamic programming](dynamic-programming.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-how-to-build-a-brain-from-scratch-course-of-the-university-of-oxford/2022/4/solution.md)
