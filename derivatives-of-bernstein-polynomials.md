# Derivatives of Bernstein polynomials

↑ **Parent:** [Bernstein polynomial](bernstein-polynomial.md)

Differentiating the Bernstein basis $p_{n,j}(x)=\binom njx^j(1-x)^{n-j}$ gives $p_{n,j}'=n(p_{n-1,j-1}-p_{n-1,j})$, with out-of-range terms zero. Telescoping coefficient differences and induction give the displayed formula, where $(n)_r=n!/(n-r)!$ and $0\le r\le n$. For $n>r$, set $g_{n,r}(t)=(n)_r\Delta_{1/n}^rf((n-r)t/n)$; then $B_n^{(r)}f=B_{n-r}g_{n,r}$. The rescaled argument compensates for the different sampling meshes.

**Table of contents**

- [Uniform convergence of Bernstein polynomial derivatives](uniform-convergence-of-bernstein-polynomial-derivatives.md)

## ↑ Ancestors (8)

1. [Bernstein polynomial](bernstein-polynomial.md)
2. [Weierstrass approximation theorem](weierstrass-approximation-theorem.md)
3. [Stone-Weierstrass theorem](stone-weierstrass-theorem.md)
4. [Functional analysis](functional-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-69/2/solution.md)
