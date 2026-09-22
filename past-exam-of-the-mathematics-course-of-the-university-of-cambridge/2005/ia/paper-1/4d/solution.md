<h1 id="4d/solution">Solution</h1>

↑ **Parent:** [4D](../4d.md)

Suppose, towards a contradiction, that $|a_nz^n|\le M$ for every $n$, where $|z|>R$. Choose a radius $\rho$ strictly between $R$ and $|z|$, and take any $w$ with $|w|=\rho$. Then

$$
|a_nw^n|=|a_nz^n|\left|\frac wz\right|^n\le M\left(\frac\rho{|z|}\right)^n.
$$

The [geometric series](../../../../../geometric-series.md) on the right converges because its ratio lies in $[0,1)$. The [comparison test for series](../../../../../comparison-test-for-series.md) therefore gives [absolute convergence](../../../../../absolute-convergence.md) of the [power series](../../../../../power-series.md) at $w$, contrary to the defining property of its [radius of convergence](../../../../../radius-of-convergence.md). Thus **$|a_nz^n|$ is unbounded in $n$ whenever $|z|>R$**. This is the [bounded power-series terms force interior absolute convergence](../../../../../bounded-power-series-terms-force-interior-absolute-convergence.md) principle. The case $R=\infty$ has no points outside its convergence disk and the assertion is vacuous there.

Every possible [radius of convergence](../../../../../radius-of-convergence.md) is realized by an explicit [power series](../../../../../power-series.md):

$$
\boxed{\begin{array}{c|c}R&\text{series}\\\hline 0&\displaystyle\sum_{n=0}^\infty n!z^n\\0<R<\infty&\displaystyle\sum_{n=0}^\infty(z/R)^n\\\infty&\displaystyle\sum_{n=0}^\infty z^n/n!\end{array}}
$$

For the first, consecutive absolute terms have ratio $(n+1)|z|$, so at every $z\ne0$ they eventually grow and do not tend to zero; at zero the series is defined. The middle [geometric series](../../../../../geometric-series.md) converges absolutely exactly for $|z|<R$, and outside that disk its terms grow. The last has consecutive-term ratio $|z|/(n+1)\to0$, so the [ratio test](../../../../../ratio-test.md) gives [absolute convergence](../../../../../absolute-convergence.md) for every finite $z$. These arguments use the necessary zero-term condition for convergence, the [comparison test for series](../../../../../comparison-test-for-series.md), and [absolute convergence](../../../../../absolute-convergence.md) of a [geometric series](../../../../../geometric-series.md) with ratio less than one; they do not assume convergence on the boundary.

## ↑ Ancestors (10)

1. [4D](../4d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
