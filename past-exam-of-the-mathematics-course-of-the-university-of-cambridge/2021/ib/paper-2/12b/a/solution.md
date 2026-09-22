<h1 id="12b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the [Taylor series](../../../../../../taylor-series.md) of the entire function as

$$
f(z)=\sum_{k=0}^{\infty}c_kz^k.
$$

The [Cauchy estimate](../../../../../../cauchy-estimate.md) on the circle $|z|=R$ gives

$$
|c_k|\leq\frac{\max_{|z|=R}|f(z)|}{R^k}
\leq aR^{n/2-k}+bR^{-k}.
$$

If $k>n/2$, letting $R\to\infty$ gives $c_k=0$. Since $n$ is odd,

$$
\boxed{\deg f\leq\lfloor n/2\rfloor}.
$$

For the second question, suppose such an $f$ existed. It never vanishes, so $g=1/f$ is analytic on $\mathbb C\setminus\{0\}$ and

$$
|g(z)|\leq\sqrt{|z|}.
$$

The [Riemann removable singularity theorem](../../../../../../riemann-removable-singularity-theorem.md) extends $g$ analytically across zero with $g(0)=0$. Applying the result just proved with $n=1$, $a=1$, and $b=0$ makes $g$ a polynomial of degree at most zero. It must then be identically zero, contradicting $g=1/f$ away from zero. Therefore no such function exists.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12B](../../12b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
