# Characteristic function under conditionally symmetric martingale increments

↑ **Parent:** [Conditionally symmetric increments](conditionally-symmetric-increments.md)

Suppose $X$ is a continuous local martingale starting at zero, with [conditionally symmetric increments](conditionally-symmetric-increments.md), and terminal conditional expectations have continuous martingale versions. Then

$$
\mathbb E e^{i\theta X_T}=\mathbb E e^{-\theta^2\langle X\rangle_T/2}.
$$

To prove this, set $M_t=\mathbb E[e^{i\theta X_T}\mid\mathcal F_t]$. Symmetry makes $e^{-2i\theta X_t}M_t$ a martingale, and the [Itô product rule](ito-product-rule.md) gives $d\langle M,X\rangle=i\theta M\,d\langle X\rangle$. Consequently $e^{-i\theta X_t-\theta^2\langle X\rangle_t/2}M_t$ is a bounded local martingale, hence a martingale. Evaluating at the endpoints proves the formula. If also $X_T\sim N(0,T)$ for all $T$, the values of the bracket [Laplace transform](laplace-transform.md) at $1$ and $2$ force $\langle X\rangle_T=T$ almost surely. Continuity and the [Lévy characterization of Brownian motion](levy-characterization-of-brownian-motion.md) then identify $X$ as [Brownian motion](brownian-motion-split.md).

## ↑ Ancestors (10)

1. [Conditionally symmetric increments](conditionally-symmetric-increments.md)
2. [Continuous local martingale](continuous-local-martingale.md)
3. [Local martingale](local-martingale.md)
4. [Continuous-time martingale](continuous-time-martingale.md)
5. [Martingale](martingale-split.md)
6. [Probability theory](probability-theory-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-25/5/d/solution.md)
