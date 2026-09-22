<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use first the test function $f(x)=x$. The assumed [martingale problem](../../../../../../martingale-problem.md) says that

$$
Y_t=X_t-X_0-\int_0^t b(X_s)\,ds
$$

is a continuous local martingale. Next use $f(x)=x^2$ to see that

$$
X_t^2-X_0^2-\int_0^t\bigl(2X_sb(X_s)+\sigma(X_s)^2\bigr)\,ds
$$

is a local martingale. On the other hand, [Itô formula](../../../../../../ito-s-lemma.md) applied to $X=X_0+\int b(X_s)ds+Y$ shows that

$$
X_t^2-X_0^2-\int_0^t2X_sb(X_s)\,ds-[Y]_t
$$

is a local martingale. Their difference is both a continuous local martingale and a finite-variation process, so

$$
[Y]_t=\int_0^t\sigma(X_s)^2\,ds.
$$

Part (b), with $H_s=\sigma(X_s)^2>0$, supplies a Brownian motion $W$ such that

$$
Y_t=\int_0^t\sigma(X_s)\,dW_s.
$$

Therefore

$$
X_t=X_0+\int_0^t b(X_s)\,ds+\int_0^t\sigma(X_s)\,dW_s,
$$

so $X$ is a [weak solution of a stochastic differential equation](../../../../../../weak-solution-of-a-stochastic-differential-equation.md) to the stated equation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
