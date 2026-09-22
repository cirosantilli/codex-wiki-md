<h1 id="7h/solution">Solution</h1>

↑ **Parent:** [7H](../7h.md)

Set

$$
p_n=\mathbb P(X_n=1\mid X_0=1).
$$

Conditioning on $X_n$ gives the affine recurrence

$$
p_{n+1}=(1-\alpha)p_n+\beta(1-p_n)
=\beta+(1-\alpha-\beta)p_n.
$$

Its fixed point is the first component of the [stationary distribution](../../../../../stationary-distribution.md),

$$
\pi_1=\frac{\beta}{\alpha+\beta}.
$$

Thus $p_n-\pi_1=(1-\alpha-\beta)^n(p_0-\pi_1)$, and $p_0=1$ gives

$$
\boxed{\mathbb P(X_n=1\mid X_0=1)
=\frac{\beta}{\alpha+\beta}
+\frac{\alpha}{\alpha+\beta}(1-\alpha-\beta)^n}.
$$

Starting instead from state two gives the same recurrence with initial value zero. Therefore

$$
\boxed{\mathbb P(X_n=1\mid X_0=2)
=\frac{\beta}{\alpha+\beta}
\left[1-(1-\alpha-\beta)^n\right]}.
$$

## ↑ Ancestors (10)

1. [7H](../7h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
