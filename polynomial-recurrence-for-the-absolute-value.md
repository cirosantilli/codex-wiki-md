# Polynomial recurrence for the absolute value

↑ **Parent:** [Weierstrass approximation theorem](weierstrass-approximation-theorem.md)

Starting with $p_0=0$ on $[-1,1]$, this [polynomial](polynomial-split.md) recurrence gives $0\le p_r(x)\le |x|$ and $p_{r+1}(x)\ge p_r(x)$. Indeed the error satisfies $|x|-p_{r+1}=(|x|-p_r)[1-(|x|+p_r)/2]$. Its pointwise limit solves $p^2=x^2$, so it is $|x|$. [Dini's theorem](dini-s-theorem.md) gives [uniform convergence](uniform-convergence.md). Each [continuous](continuous-function.md) [piecewise linear function](piecewise-linear-function.md) is an affine function plus a finite [linear combination](linear-combination.md) of $(x-t)_+=(x-t+|x-t|)/2$. Scaling and translating the recurrence therefore gives [polynomial approximation](polynomial-approximation.md) of every such function, and their density gives the [Weierstrass approximation theorem](weierstrass-approximation-theorem.md).

## ↑ Ancestors (7)

1. [Weierstrass approximation theorem](weierstrass-approximation-theorem.md)
2. [Stone-Weierstrass theorem](stone-weierstrass-theorem.md)
3. [Functional analysis](functional-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-58/6/solution.md)
