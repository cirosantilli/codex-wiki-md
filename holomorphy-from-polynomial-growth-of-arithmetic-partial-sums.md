# Holomorphy from polynomial growth of arithmetic partial sums

↑ **Parent:** [Dirichlet series](dirichlet-series.md)

Let $S(x)=\sum_{n\le x}a_n$ satisfy $|S(x)|\le Cx^\alpha$ for $x\ge1$. The [Abel summation formula](abel-s-summation-formula.md) gives $A(s)=s\int_1^\infty S(t)t^{-s-1}dt$ when $\operatorname{Re}s>\alpha$, since its finite-sum boundary term tends to zero. Split this integral into blocks $I_m(s)=\int_m^{m+1}S(t)t^{-s-1}dt$. For every $\delta>0$, the estimate $|I_m(s)|\le Cm^{-1-\delta}$ holds uniformly on $\operatorname{Re}s>\alpha+\delta$. Each block is an [entire function](entire-function.md), by differentiation under the finite-range integral on compact sets. The [Weierstrass M-test](weierstrass-m-test.md) makes their sum locally uniformly convergent and therefore [holomorphic](holomorphic-function-split.md); multiplication by $s$ preserves holomorphy.

This proof distinguishes uniform convergence of the block sum on a whole half-plane from local uniform convergence after multiplication by $s$. The latter is all that holomorphy needs. In particular, a bound $\sum_{n\le x}\mu(n)=O(x^\alpha)$ gives a holomorphic continuation of the reciprocal [Riemann zeta function](riemann-zeta-function.md) to this half-plane and excludes zeta zeros there, with the pole at one treated by cancellation.

## ↑ Ancestors (6)

1. [Dirichlet series](dirichlet-series.md)
2. [Analytic number theory](analytic-number-theory-split.md)
3. [Number theory](number-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford/2007/a/2/solution.md)
