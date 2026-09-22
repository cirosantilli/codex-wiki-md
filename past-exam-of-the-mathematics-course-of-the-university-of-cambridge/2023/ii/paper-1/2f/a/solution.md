<h1 id="2f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Liouville approximation theorem](../../../../../../liouville-approximation-theorem.md) states that if $\alpha$ is an irrational algebraic number of degree $d\geq2$, then there is a constant $c(\alpha)>0$ such that every reduced rational $p/q$ satisfies

$$
\boxed{\left|\alpha-\frac pq\right|>
\frac{c(\alpha)}{q^d}}.
$$

Let $P\in\mathbb Z[X]$ be the [minimal polynomial](../../../../../../minimal-polynomial.md) of $\alpha$, of degree $d$. Since $P$ is irreducible of degree greater than one, $P(p/q)\ne0$. Moreover,

$$
q^dP(p/q)\in\mathbb Z\setminus\{0\},
$$

and hence

$$
|P(p/q)|\geq q^{-d}.
$$

On the compact interval $I=[\alpha-1,\alpha+1]$, put

$$
M=\max_{x\in I}|P'(x)|.
$$

If $p/q\in I$, the [mean value theorem](../../../../../../mean-value-theorem.md) gives a point $\xi$ between $\alpha$ and $p/q$ such that

$$
|P(p/q)|=|P'(\xi)|\left|\frac pq-\alpha\right|
\leq M\left|\frac pq-\alpha\right|.
$$

Thus $|\alpha-p/q|\geq M^{-1}q^{-d}$. If $p/q\notin I$, then $|\alpha-p/q|>1\geq q^{-d}$. Taking any

$$
0<c(\alpha)<\min\{1,M^{-1}\}
$$

proves the stated strict inequality.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2F](../../2f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
