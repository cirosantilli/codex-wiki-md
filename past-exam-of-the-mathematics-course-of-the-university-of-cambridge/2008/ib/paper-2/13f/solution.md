<h1 id="13f/solution">Solution</h1>

↑ **Parent:** [13F](../13f.md)

Because $|u_n(x)|\le M_n$ and the numerical series converges, its tails can be made arbitrarily small independently of $x$:

$$
\sup_{x\in E}\left|\sum_{n=N+1}^M u_n(x)\right|\le\sum_{n>N}M_n\longrightarrow0.
$$

Thus the partial sums satisfy the uniform Cauchy criterion; completeness of the real numbers supplies the pointwise limit, and the same tail bound proves [uniform convergence](../../../../../uniform-convergence.md). This is the [Weierstrass M-test](../../../../../weierstrass-m-test.md).

For $E_R$ with $R>0$, choose an integer $N>2R$. If $n>N$ and $|x|<R$, then $|x\pm n|\ge n-R>n/2$, so $|u_n(x)|\le8/n^2$. The tail is therefore uniformly convergent by the M-test; adding its finitely many earlier terms preserves [uniform convergence](../../../../../uniform-convergence.md), even though those earlier terms can be unbounded near excluded integers. For $R\le0$ the set is empty and the claim is vacuous.

Each summand is continuous on $E=\mathbb R\setminus\mathbb Z$. Around any $x\in E$, choose an interval containing $x$, avoiding integers and lying in some $E_R$. The uniform-limit [continuity](../../../../../continuous-function.md) theorem then proves $\boxed{f\text{ is continuous on }E}$.

The series is **not uniformly convergent on all of $E$**. [Uniform convergence](../../../../../uniform-convergence.md) would require $u_n\to0$ uniformly, but $u_n(n+1/2)\ge4$ for every $n>0$. These evaluation points belong to $E$, contradicting that necessary condition.

## ↑ Ancestors (10)

1. [13F](../13f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
