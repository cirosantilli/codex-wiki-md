<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

There is a missing hypothesis in the original PDF: $k$ must be a [splitting field for finite group representations](../../../../../../splitting-field-for-finite-group-representations.md). For example,

$$
\mathbb F_2C_3\cong\mathbb F_2[X]/(X^3-1)\cong\mathbb F_2\times\mathbb F_4,
$$

because $X^3-1=(X-1)(X^2+X+1)$ and the quadratic factor is irreducible. This algebra has two [simple modules](../../../../../../irreducible-module.md), whereas $C_3$ has three conjugacy classes, all $2$-regular. Thus the printed assertion for an arbitrary [field](../../../../../../field.md) is false.

Under the intended splitting hypothesis, fix compatible lifts defining [Brauer characters](../../../../../../brauer-character.md). Let $\mathcal K_{p'}$ be the set of conjugacy classes of [p-regular elements](../../../../../../p-regular-element.md). Character additivity and the tensor-product formula define the unital algebra homomorphism

$$
\Phi:\mathbb C\otimes_{\mathbb Z}R_k(G)\longrightarrow\prod_{C\in\mathcal K_{p'}}\mathbb C,\qquad z\otimes[V]\longmapsto\bigl(z\chi_V(g_C)\bigr)_C.
$$

We use the [Brauer character basis theorem](../../../../../../brauer-character-basis-theorem.md): over a splitting [field](../../../../../../field.md) the irreducible [Brauer characters](../../../../../../brauer-character.md) form a complex basis of the [class functions](../../../../../../class-function.md) on the p-regular conjugacy classes. Therefore $\Phi$ maps the basis $1\otimes[S]$ bijectively to a basis and is an algebra isomorphism. Comparing dimensions gives

$$
\boxed{\mathbb C\otimes R_k(G)\cong\mathbb C^{\mathcal K_{p'}},\qquad\#\{\text{simple }kG\text{-modules}\}=|\mathcal K_{p'}|\quad(k\text{ splitting})}.
$$

Isomorphism classes are understood in the count.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 138](../../../paper-138-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
