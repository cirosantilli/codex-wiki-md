<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Differentiate the conditional identity from part a. To justify doing so, fix a compact parameter interval $|\lambda|\leq L$. Every $n$th derivative of $M_\lambda(t)$ is a polynomial in $B_t,t,$ and $\lambda$ times $M_\lambda(t)$, and its absolute value is bounded by

$$
C_{n,L,t}(1+|B_t|^n)e^{(L+1)|B_t|}.
$$

This bound is integrable because a Gaussian random variable has every polynomially weighted exponential moment. Dominated differentiation of conditional expectation therefore gives

$$
\mathbb E\left[\frac{\partial^nM_\lambda(t)}{\partial\lambda^n}\,\middle|\,\mathcal F_s\right]
=\frac{\partial^nM_\lambda(s)}{\partial\lambda^n}.
$$

**Thus every [parameter derivative of the exponential Brownian martingale](../../../../../../parameter-derivative-of-the-exponential-brownian-martingale.md) is itself a martingale.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
