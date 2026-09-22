<h1 id="9d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

All three examples below have [radius of convergence](../../../../../../radius-of-convergence.md) one, because the $n$th roots of their coefficient moduli tend to one.

For convergence everywhere on the boundary, take **$\sum_{n=1}^\infty z^n/n^2$**. On $|z|=1$ it converges absolutely: for $n\ge2$, $1/n^2\le1/[n(n-1)]=1/(n-1)-1/n$, whose sum telescopes to a finite value.

For divergence everywhere on the boundary, take **$\sum_{n=0}^\infty z^n$**. If $|z|=1$, every term has modulus one, so the [term test for divergence](../../../../../../term-test-for-divergence.md) applies.

For mixed boundary behavior, take **$\sum_{n=1}^\infty z^n/n$**. At $z=1$ it is the divergent [harmonic series](../../../../../../harmonic-series.md); each successive dyadic block contributes at least $1/2$. At every other point $|z|=1$, [summation by parts](../../../../../../abel-s-summation-formula.md) proves convergence. Indeed put $B_k=\sum_{j=m}^kz^j$, so the finite [geometric series](../../../../../../geometric-series.md) gives $|B_k|\le2/|1-z|=:C_z$. Then

$$
\sum_{n=m}^N\frac{z^n}{n}=\frac{B_N}{N}+\sum_{n=m}^{N-1}B_n\left(\frac1n-\frac1{n+1}\right),\qquad
\left|\sum_{n=m}^N\frac{z^n}{n}\right|\le\frac{C_z}{m}.
$$

Thus the partial sums form a [Cauchy sequence](../../../../../../cauchy-sequence.md) and converge. This derives the relevant [Dirichlet test](../../../../../../dirichlet-test.md) rather than only naming it.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [9D](../../9d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
