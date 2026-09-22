<h1 id="4/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $W$ be a Brownian motion, set $X=W$, and define

$$
B_t=\int_0^t\operatorname{sign}(W_s)dW_s.
$$

This is a continuous local martingale with quadratic variation $t$, hence is Brownian by the [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md). Since $\operatorname{sign}^2=1$,

$$
dX_t=dW_t=\operatorname{sign}(X_t)dB_t,
$$

which gives a weak solution.

Suppose a strong solution existed. It has quadratic variation $t$, so $X$ itself is Brownian. The supplied [Tanaka formula](../../../../../../tanaka-s-formula.md) gives $|X_t|=B_t+L_t$, and $L$ is adapted to the completed filtration of $|X|$. Hence $B$ and $|X|$ generate the same completed filtration. Strongness would make $X$, and therefore $\operatorname{sign}(X_t)$, measurable with respect to the history of $|X|$. But a Brownian excursion has an independent symmetric sign; in particular, conditionally on the reflected Brownian path, the sign at a fixed nonzero time is not measurable. This contradiction proves that **no strong solution exists**.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [4](../../4.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
