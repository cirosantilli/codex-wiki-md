# Power-law crossover in a singular perturbation

↑ **Parent:** [Singular perturbation](singular-perturbation-split.md)

For $\epsilon>0$, the two terms in $y=x^{-1/\epsilon}+x$ are equal at $x=1$. Their ratio is larger than one for $0<x<1$ and smaller than one for $x>1$. As $\epsilon\to0^+$ it tends to infinity at fixed $x<1$ and to zero at fixed $x>1$. Comparable contributions require $|\log x|=O(\epsilon)$, equivalently $x=1+O(\epsilon)$.

To resolve this region exactly, introduce the [inner variable](inner-variable.md) $X=\log x/\epsilon$. Then $y=e^{-X}+e^{\epsilon X}\sim e^{-X}+1$ for bounded $X$. At fixed $x>1$, the first term $\exp[-(\log x)/\epsilon]$ is smaller than every positive integer power of $\epsilon$, so a [regular perturbation](regular-perturbation.md) in powers of $\epsilon$ misses it. At fixed $x<1$, that same term diverges. This explains why a [power series](power-series.md) approximation valid on one side need not be a uniform approximation across the crossover.

## ↑ Ancestors (7)

1. [Singular perturbation](singular-perturbation-split.md)
2. [Ordinary differential equation](ordinary-differential-equation.md)
3. [Differential equation](differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-differential-equations-2-course-of-the-university-of-oxford/2021/3/b/solution.md)
