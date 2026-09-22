<h1 id="17b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Here

$$
\phi(u,h)=\frac14\left[
f(u)+3f\left(u+\frac{2h}{3}f(u)\right)\right].
$$

For $0<h\leq1$, the Lipschitz bound on $f$ gives

$$
|\phi(u,h)-\phi(v,h)|
\leq\left(K+\frac{K^2}{2}\right)|u-v|,
$$

so part (ii) applies with a constant independent of sufficiently small $h$.

The exact solution has the [Taylor expansion](../../../../../../taylor-series.md)\>

$$
y(t+h)=y(t)+hf(y(t))
+\frac{h^2}{2}f'(y(t))f(y(t))+O(h^3).
$$

Meanwhile,

$$
f\left(y+\frac{2h}{3}f(y)\right)
=f(y)+\frac{2h}{3}f'(y)f(y)+O(h^2),
$$

so one numerical step from $y$ is

$$
y+h\phi(y,h)
=y+hf(y)+\frac{h^2}{2}f'(y)f(y)+O(h^3).
$$

The local error is therefore $O(h^3)$. Taking $p=2$ in part (ii) proves the required second-order global-error bound. This method is a two-stage [Runge-Kutta method](../../../../../../runge-kutta-method.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [17B](../../17b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
