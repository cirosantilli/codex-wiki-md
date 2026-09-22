<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $\sigma>1$, put $F(s)=-\zeta'(s)/\zeta(s)$. Its absolutely convergent [Dirichlet series](../../../../../../dirichlet-series.md) and

$$
3+4\cos\theta+\cos2\theta=2(1+\cos\theta)^2\geq0
$$

give the [three-four-one zero-free-region argument](../../../../../../three-four-one-zero-free-region-argument.md)

$$
3F(\sigma)+4\Re F(\sigma+it)+\Re F(\sigma+2it)\geq0.
$$

The pole of $\zeta$ at one gives

$$
F(\sigma)=\frac1{\sigma-1}+O(1).
$$

Suppose $\rho=\beta+i\gamma$ is a zero with $\gamma\geq4$ and $\beta$ close to one. Apply the supplied [Local partial-fraction expansion of the Riemann zeta logarithmic derivative](../../../../../../local-partial-fraction-expansion-of-the-riemann-zeta-logarithmic-derivative.md) at $\sigma+i\gamma$. Every term has positive real part, so retaining the term belonging to $\rho$ gives

$$
\Re F(\sigma+i\gamma)
\leq-\frac1{\sigma-\beta}+O(\log\gamma).
$$

At $\sigma+2i\gamma$ the same expansion gives merely $\Re F(\sigma+2i\gamma)\leq O(\log\gamma)$. The zero is included in the supplied disk whenever $1-\beta$ and $\sigma-1$ are sufficiently small. Hence

$$
0\leq\frac3{\sigma-1}-\frac4{\sigma-\beta}+O(\log\gamma).
$$

Set $L=\log\gamma$ and $\sigma=1+a/L$, where $a>0$ is a sufficiently small fixed constant. If $(1-\beta)L$ were smaller than a sufficiently small constant $c>0$, division by $L$ would give

$$
0\leq\frac3a-\frac4{a+(1-\beta)L}+O(1)<0,
$$

a contradiction. Conjugation handles negative $\gamma$. Reducing $c$ to absorb the bounded range proves the classical [zero-free region of the Riemann zeta function](../../../../../../zero-free-region-of-the-riemann-zeta-function.md)

$$
\boxed{\zeta(s)\ne0\quad\text{for}\quad
\sigma\geq1-\frac c{\log|t|},\quad |t|\geq4}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
