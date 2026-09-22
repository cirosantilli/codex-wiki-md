<h1 id="10f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The continuity of the [cumulative distribution function](../../../../../../cumulative-distribution-function.md) gives the [probability integral transform](../../../../../../probability-integral-transform.md): $F(X_i)$ is uniform on $[0,1]$. Strict monotonicity or a [probability](../../../../../../probability.md) density for $F$ is not required. Since $F$ is nondecreasing,

$$
U=F(Y_n)=\max_{1\leq i\leq n}F(X_i).
$$

By [independence](../../../../../../independent-random-variables.md), $P(U\leq u)=u^n$ for $0\leq u\leq1$, so $U$ has [probability density function](../../../../../../probability-density-function.md) $nu^{n-1}$. Average the conditional [probability](../../../../../../probability.md) in part (b) using this distribution:

$$
P(\tau=k)=n\int_0^1u^{k+n-2}(1-u)\,du
=n\left(\frac1{k+n-1}-\frac1{k+n}\right).
$$

Thus **$\boxed{P(\tau=k)=n/[(k+n-1)(k+n)]}$**. The expression telescopes to total mass one, so the waiting time is finite almost surely.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
