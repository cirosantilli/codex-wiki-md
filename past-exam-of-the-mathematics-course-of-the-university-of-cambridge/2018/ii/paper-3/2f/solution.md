<h1 id="2f/solution">Solution</h1>

↑ **Parent:** [2F](../2f.md)

One form of the [Baire category theorem](../../../../../baire-category-theorem.md) says that a nonempty [complete metric space](../../../../../complete-metric-space.md) cannot be a countable union of closed [nowhere dense sets](../../../../../nowhere-dense-set.md).

For each nonnegative integer $n$, put

$$
Z_n=\{z\in\mathbb C:f^{(n)}(z)=0\}.
$$

Because $f$ is an [entire function](../../../../../entire-function.md), every [derivative](../../../../../derivative.md) $f^{(n)}$ is continuous and $Z_n$ is closed. No $f^{(n)}$ is identically zero: if $f^{(n)}\equiv0$ for some $n$, repeated integration shows that $f$ is a [polynomial](../../../../../polynomial-split.md). By the [identity theorem](../../../../../identity-theorem.md), the zero set of the nonzero [holomorphic function](../../../../../holomorphic-function.md) $f^{(n)}$ has empty interior. Thus each $Z_n$ is [nowhere dense](../../../../../nowhere-dense-set.md).

The [complex plane](../../../../../complex-plane.md) is complete, so the [Baire category theorem](../../../../../baire-category-theorem.md) gives

$$
\mathbb C\ne\bigcup_{n=0}^{\infty}Z_n.
$$

Choose $z_0$ outside this union. Then $f^{(n)}(z_0)\ne0$ for every $n$, and hence every coefficient $f^{(n)}(z_0)/n!$ in the [Taylor series](../../../../../taylor-series.md) about $z_0$ is nonzero. **Such a point $z_0$ therefore exists.**

## ↑ Ancestors (10)

1. [2F](../2f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
