<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the fixed degree-two [irreducible polynomial](../../../../../../irreducible-polynomial.md) $f$, a [matrix](../../../../../../matrix.md) with [minimal polynomial](../../../../../../minimal-polynomial.md) a power of $f$ has only one primary component. Its [conjugacy classes](../../../../../../conjugacy-class.md) correspond to [integer partitions](../../../../../../integer-partition.md) $\lambda$ of $m$. By the [primary matrix centralizer formula](../../../../../../primary-matrix-centralizer-formula.md), its [centralizer](../../../../../../centralizer.md) has exactly the same order $c_\lambda(q^2)$ as the [centralizer](../../../../../../centralizer.md) of the corresponding [unipotent matrix](../../../../../../unipotent-matrix.md) in $GL_m(q^2)$.

Sum the [conjugacy class](../../../../../../conjugacy-class.md) sizes:

$$
\#\{g\in GL_{2m}(q):\mu_g=f^a\text{ for some }a\ge1\}
=|GL_{2m}(q)|\sum_{\lambda\vdash m}\frac1{c_\lambda(q^2)}.
$$

The same sum times $|GL_m(q^2)|$ is the number of [unipotent matrices](../../../../../../unipotent-matrix.md) of $GL_m(q^2)$, which 5(c) shows is $(q^2)^{m^2-m}$. Hence [counting matrices with a fixed primary polynomial](../../../../../../counting-matrices-with-a-fixed-primary-polynomial.md) gives

$$
\boxed{q^{2m^2-2m}\frac{|GL_{2m}(q)|}{|GL_m(q^2)|}.}
$$

In particular the exponent $a$ of the minimal polynomial is not fixed in advance: summing all [integer partitions](../../../../../../integer-partition.md) includes every possible largest block size. The usual statement takes $m\ge1$; dimension zero can instead be included with its identity convention.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
