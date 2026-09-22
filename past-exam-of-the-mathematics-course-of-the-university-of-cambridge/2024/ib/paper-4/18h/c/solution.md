<h1 id="18h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Every $x_0\in[1,\infty)$ works. Indeed, $x_1\geq\sqrt a$, and whenever $x_k\geq\sqrt a$,

$$
0\leq x_{k+1}-\sqrt a
=\frac{(x_k-\sqrt a)^2}{2x_k}
\leq x_k-\sqrt a.
$$

The iterates from $k=1$ onward therefore decrease to a [limit](../../../../../../limit-of-a-function.md), and the recurrence forces that [limit](../../../../../../limit-of-a-function.md) to be $\sqrt a$.

There is also an explicit error bound. Put

$$
q=\left|\frac{x_0-\sqrt a}{x_0+\sqrt a}\right|<1.
$$

A direct calculation gives

$$
\frac{x_{k+1}-\sqrt a}{x_{k+1}+\sqrt a}
=\left(\frac{x_k-\sqrt a}{x_k+\sqrt a}\right)^2.
$$

Hence, for $k\geq1$,

$$
\boxed{
|x_k-\sqrt a|
=\frac{2\sqrt a\,q^{2^k}}{1-q^{2^k}}
\leq\frac{2\sqrt a}{1-q}q^{2^k}}.
$$

This double-exponential decay is consistent with the Newton bound in part (a). For the chosen objective, the supplied factorization also gives

$$
f(x)-f(\sqrt a)
=\frac13(x-\sqrt a)^2(x+2\sqrt a),
$$

so convergence of the objective and convergence of the iterates are equivalent on $[1,\infty)$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18H](../../18h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
