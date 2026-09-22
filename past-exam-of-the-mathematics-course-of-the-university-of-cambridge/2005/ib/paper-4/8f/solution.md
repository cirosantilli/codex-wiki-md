<h1 id="8f/solution">Solution</h1>

↑ **Parent:** [8F](../8f.md)

An $n$-node [Gaussian quadrature](../../../../../gaussian-quadrature.md) formula chooses nodes and weights for an integral with a positive weight so that every [polynomial](../../../../../polynomial-split.md) of degree at most $2n-1$ is integrated exactly. Its nodes are the zeros of the degree-$n$ [orthogonal polynomial](../../../../../orthogonal-polynomial.md) for that weight.

For the even weight $w(x)=1-x^2$, the monic orthogonal quadratic has the form $p_2(x)=x^2-d$. Orthogonality to $x$ follows from oddness; orthogonality to one gives

$$
d=\frac{\int_{-1}^1x^2(1-x^2)dx}{\int_{-1}^1(1-x^2)dx}=\frac{4/15}{4/3}=\frac15.
$$

The nodes are $\pm1/\sqrt5$. The equal weights sum to $4/3$, hence each is $2/3$. The [two-node Gaussian quadrature with quadratic weight](../../../../../two-node-gaussian-quadrature-with-quadratic-weight.md) is therefore

$$
\boxed{\int_{-1}^1(1-x^2)f(x)dx\simeq\frac23\left[f(-1/\sqrt5)+f(1/\sqrt5)\right].}
$$

To verify cubic exactness, divide any cubic as $P=p_2Q+R$ with $\deg Q,\deg R\leq1$. Orthogonality removes $p_2Q$ from the integral and its nodal values vanish; linear interpolation integrates $R$ exactly. This also proves the Gaussian property rather than merely matching two moments.

## ↑ Ancestors (10)

1. [8F](../8f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
