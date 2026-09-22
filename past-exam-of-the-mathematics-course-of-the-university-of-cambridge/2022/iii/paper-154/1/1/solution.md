<h1 id="1/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Choose a [test function](../../../../../../space-of-test-functions.md) $\chi$ that equals one on the unit ball and vanishes outside the ball of radius two. Since

$$
\operatorname{div}(x\chi)=d\chi+x\mathbin{\cdot}\nabla\chi,
$$

[integration by parts](../../../../../../integration-by-parts.md) gives

$$
d\int\chi u^2
=-\int(x\mathbin{\cdot}\nabla\chi)u^2-2\int\chi u\,x\mathbin{\cdot}\nabla u.
$$

The first term on the right is supported where $1\leq|x|\leq2$, where $u^2\leq |x|^\alpha u^2$. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and [Young inequality](../../../../../../young-s-inequality-for-products.md) bound the second term by

$$
2\left|\int\chi u\,x\mathbin{\cdot}\nabla u\right|
\leq\frac d2\int\chi u^2+C\int|\nabla u|^2.
$$

After absorbing the first integral,

$$
\int_{|x|\leq1}|u|^2
\leq C\left(\int|\nabla u|^2+\int|x|^\alpha|u|^2\right)
=C\|u\|_\Sigma^2.
$$

This estimate also proves completeness. Indeed, a [Cauchy sequence](../../../../../../cauchy-sequence.md) in $\Sigma$ is Cauchy in $H^1$ locally, while its gradients and the functions $|x|^{\alpha/2}u_n$ converge in $L^2$. The limits agree locally with a function $u$, so $u\in\Sigma$ and $u_n\to u$ in the energy norm. Thus $\Sigma$ is a [Hilbert space](../../../../../../hilbert-space-split.md); it is the [confining-potential energy space](../../../../../../confining-potential-energy-space.md) for $V(x)=|x|^\alpha$.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [1](../../1.md)
3. [Paper 154](../../../paper-154-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
