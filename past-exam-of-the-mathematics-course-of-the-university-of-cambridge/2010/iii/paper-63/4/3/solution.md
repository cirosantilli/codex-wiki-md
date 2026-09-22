<h1 id="4/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [collocation order theorem](../../../../../../collocation-order-theorem.md) identifies the classical order with the order of its interpolatory quadrature. If $\sum_i b_i g(c_i)$ integrates every [polynomial](../../../../../../polynomial-split.md) of degree at most $p-1$ exactly, but fails for some [polynomial](../../../../../../polynomial-split.md) of degree $p$, then the collocation method has order $p$ for sufficiently smooth differential equations and the local implicit stage branch. With $s$ nodes, $s\le p\le2s$.

Equivalently, put $\pi_s(\tau)=\prod_i(\tau-c_i)$. If its first $k$ moments vanish,

$$
\int_0^1\tau^j\pi_s(\tau)d\tau=0\quad(0\le j<k),
$$

and the next does not, then $p=s+k$. [Polynomial](../../../../../../polynomial-split.md) division explains the quadrature part: any [polynomial](../../../../../../polynomial-split.md) through degree $s+k-1$ is a remainder of degree below $s$ plus $\pi_s$ times a [polynomial](../../../../../../polynomial-split.md) of degree below $k$. The remainder is integrated exactly by interpolation, and the remaining integral vanishes. Conversely a nonzero next moment is an explicit failed quadrature test. The differential-equation order assertion is the collocation theorem being stated here. In particular [Gauss collocation methods](../../../../../../gauss-legendre-method.md) achieve $2s$, [Radau IIA methods](../../../../../../radau-iia-method.md) achieve $2s-1$, and endpoint-including [Lobatto IIIA methods](../../../../../../lobatto-iiia-method.md) achieve $2s-2$ for $s\ge2$.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [4](../../4.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
