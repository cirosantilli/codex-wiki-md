# Feynman-Kac formula with a bounded potential

↑ **Parent:** [Feynman-Kac formula](feynman-kac-formula.md)

For bounded $V$ and bounded initial data $f$, a sufficiently regular [classical solution](classical-solution.md) bounded on every finite time slab satisfies

$$
u(t,x)=\mathbb E_x\left[f(B_t)\exp\!\left(\int_0^tV(B_s)ds\right)\right].
$$

To prove this, the [Itô formula](ito-s-lemma.md) and [Itô product rule](ito-product-rule.md) make $u(T-t,B_t)e^{\int_0^tV(B_s)ds}$ a [local martingale](local-martingale.md). Its deterministic bound on $[0,T]$ makes it a true [martingale](martingale-split.md); taking [expectations](expected-value.md) at the two endpoints gives the formula. This also gives uniqueness in the finite-horizon bounded class. The exponent has the same sign as the potential in the equation.

**Table of contents**

- [Soft killing limit for Brownian nonnegative survival](soft-killing-limit-for-brownian-nonnegative-survival.md)
- [Zero-noise limit with a bounded potential](zero-noise-limit-with-a-bounded-potential.md)
- [Positive-potential growth from Brownian recurrence](positive-potential-growth-from-brownian-recurrence.md)

## ↑ Ancestors (10)

1. [Feynman-Kac formula](feynman-kac-formula.md)
2. [Kolmogorov backward equation](kolmogorov-backward-equation.md)
3. [Stochastic differential equation](stochastic-differential-equation.md)
4. [Stochastic calculus](stochastic-calculus-split.md)
5. [Stochastic process](stochastic-process-split.md)
6. [Probability theory](probability-theory-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-33/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-202/6/b/solution.md)
- [Positive-potential growth from Brownian recurrence](positive-potential-growth-from-brownian-recurrence.md)
