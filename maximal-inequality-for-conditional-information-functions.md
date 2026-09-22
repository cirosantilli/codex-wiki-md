# Maximal inequality for conditional information functions

↑ **Parent:** [Conditional information function](conditional-information-function.md)

For increasing [sigma-algebras](sigma-algebra.md) $\mathcal G_n$, put $f_n=I_\mu(\xi\mid\mathcal G_n)$ and $F=\sup_n f_n$. For each atom $A\in\xi$ and $t\geq0$,

$$
\mu(A\cap\{F>t\})\leq e^{-t}.
$$

Together with the bound by $\mu(A)$ and the [tail integral formula for moments](tail-integral-formula-for-moments.md), this yields $\int F\,d\mu\leq H_\mu(\xi)+1$. The inequality follows by stopping the [conditional-expectation martingale](conditional-expectation-martingale.md) $\mathbb E[\mathbf1_A\mid\mathcal G_n]$ the first time it falls below $e^{-t}$.

## ↑ Ancestors (9)

1. [Conditional information function](conditional-information-function.md)
2. [Entropy of a countable measurable partition](entropy-of-a-countable-measurable-partition.md)
3. [Measurable partition](measurable-partition.md)
4. [Measure theory](measure-theory-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-108/3/solution.md)
- [Shannon-McMillan-Breiman theorem](shannon-mcmillan-breiman-theorem.md)
