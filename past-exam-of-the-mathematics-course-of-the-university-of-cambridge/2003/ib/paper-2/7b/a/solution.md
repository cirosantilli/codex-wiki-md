<h1 id="7b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take the unit circle counterclockwise and $n\ge0$. The integrand is a Laurent [polynomial](../../../../../../polynomial-split.md) with its only possible singularity at zero. Its expansion is

$$
\frac1z(z-z^{-1})^{2n}
=\sum_{j=0}^{2n}(-1)^j\binom{2n}{j}z^{2n-2j-1}.
$$

The $z^{-1}$ term is the term $j=n$, so the [residue](../../../../../../residue.md) is $(-1)^n\binom{2n}{n}$. The [residue theorem](../../../../../../residue-theorem.md) gives

$$
\boxed{\oint_{|z|=1}(z-z^{-1})^{2n}\frac{dz}{z}
=2\pi i(-1)^n\frac{(2n)!}{(n!)^2}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7B](../../7b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
