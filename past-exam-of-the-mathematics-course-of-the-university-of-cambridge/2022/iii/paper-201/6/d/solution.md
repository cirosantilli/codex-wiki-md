<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $N(ds,dy)$ be a Poisson random measure on $(0,\infty)^2$ with intensity $ds\,K(dy)$ and define

$$
X_t=\int_{(0,t]\times(0,\infty)}y\,N(ds,dy).
$$

The assumption $\int yK(dy)<\infty$ makes this integral finite on compact time intervals. The exponential formula for a Poisson random measure gives

$$
\mathbb Ee^{iuX_t}
=\exp\left\{t\int_{(0,\infty)}(e^{iuy}-1)K(dy)\right\},
$$

so $X$ is a Lévy process with exponent $\psi$.

Choose finite-valued measurable functions $q_n\geq0$ which vanish off $[1/n,n]$ and satisfy

$$
\int|q_n(y)-y|K(dy)\longrightarrow0.
$$

This is possible by truncation followed by approximation by simple functions. Put

$$
X_t^n=\int_{(0,t]\times(0,\infty)}q_n(y)\,N(ds,dy).
$$

The measure of the support of $q_n$ is finite, and $q_n$ takes finitely many values, so $X^n$ is a simple pure-jump Lévy process. Under this common coupling,

$$
\boxed{\mathbb E\sup_{s\leq t}|X_s^n-X_s|
\leq\mathbb E\int_{(0,t]\times(0,\infty)}
|q_n(y)-y|\,N(ds,dy)
=t\int|q_n-y|\,dK\longrightarrow0.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
