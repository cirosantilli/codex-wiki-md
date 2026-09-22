<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $X_t=N_t^+-N_t^-$, where $N^+$ and $N^-$ are independent [Poisson processes](../../../../../../poisson-process.md) of rate $\lambda$. This [symmetric Poisson difference process](../../../../../../symmetric-poisson-difference-process.md) is centered, has jumps $\pm1$, and has variance rate $\sigma^2=2\lambda$. If $a,b$ are positive integers, then $X_T\in\{-a,b\}$ exactly. Optional sampling of the martingale $X_t$ gives

$$
\mathbb P(X_T=b)=\frac{a}{a+b},
\qquad
\mathbb P(X_T=-a)=\frac{b}{a+b}.
$$

Consequently

$$
\mathbb E[X_T^2]
=b^2\frac{a}{a+b}+a^2\frac{b}{a+b}
=ab.
$$

Part (d) now gives the [mean exit time](../../../../../../expected-value.md)

$$
\boxed{\mathbb E T=\frac{ab}{2\lambda}.}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [6](../../6.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
