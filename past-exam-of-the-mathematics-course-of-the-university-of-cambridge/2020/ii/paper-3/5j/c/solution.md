<h1 id="5j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [hat matrix](../../../../../../hat-matrix.md) $P$ is an [orthogonal projection](../../../../../../orthogonal-projection.md) of rank $p$, so $I-P$ is an orthogonal projection of rank $n-p$. Because $\varepsilon/\sigma$ is a standard [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md) vector, [Cochran's theorem](../../../../../../cochran-s-theorem.md) gives

$$
\frac{n\widehat\sigma^2}{\sigma^2}
=\frac{\|(I-P)\varepsilon\|^2}{\sigma^2}
\sim\chi^2_{n-p}.
$$

Thus $\widehat\sigma^2\overset d=(\sigma^2/n)\chi^2_{n-p}$. Substituting this into the preceding formula gives the [Distribution of the Akaike information criterion in a normal linear model](../../../../../../distribution-of-the-akaike-information-criterion-in-a-normal-linear-model.md):

$$
\boxed{\operatorname{AIC}\overset d=
n\log(\chi^2_{n-p})
+n\bigl(\log(2\pi\sigma^2/n)+1\bigr)+2(p+1).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5J](../../5j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
