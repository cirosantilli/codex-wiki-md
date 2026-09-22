<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose basepoints and replace the spaces and map by [CW complex](../../../../../../cw-complex.md) models. If the hypothesis is stated for unreduced [represented homology theory](../../../../../../represented-homology-theory.md), the basepoint coefficient summands split naturally, so it also gives an isomorphism in reduced [represented homology theory](../../../../../../represented-homology-theory.md). Let $C$ be the homotopy [mapping cone](../../../../../../mapping-cone-homological-algebra.md) of $f$. Its reduced [represented homology theory](../../../../../../represented-homology-theory.md) is zero in every degree, by the exact sequence of the corresponding [cofiber sequence of spectra](../../../../../../cofiber-sequence-of-spectra.md).

The [mapping cone](../../../../../../mapping-cone-homological-algebra.md) $C$ is a [simply connected space](../../../../../../simply-connected-space.md): the mapping cylinder retracts onto $Z$, and coning off the path-connected space $Y$ adds no fundamental-group generators; the van Kampen calculation gives the quotient of $\pi_1Z$ by the image of $\pi_1Y$, which is trivial. Suppose some positive-degree integral [homology](../../../../../../homology-split.md) group of $C$ were nonzero, and let $n$ be the least such degree. Then $n\ge2$. Starting with $\pi_1C=0$, the [Hurewicz theorem](../../../../../../hurewicz-theorem.md) shows inductively that $\pi_iC=0$ for $i<n$: at each first possible degree $i$, its [homotopy group](../../../../../../homotopy-group.md) is identified with the zero group $H_i(C;\mathbb Z)$. It then identifies

$$
\pi_nC\cong H_n(C;\mathbb Z)\ne0.
$$

Applying the result of part (a) to the $(n-1)$-connected [based space](../../../../../../based-space.md) $C$ gives $\widetilde E_n(C)\cong\pi_nC\ne0$, contradicting the vanishing of its [represented homology theory](../../../../../../represented-homology-theory.md).

Thus $C$ is integrally acyclic, and the ordinary [homology](../../../../../../homology-split.md) exact sequence says that $f$ is an integral homology isomorphism. The allowed [homological Whitehead theorem](../../../../../../homological-whitehead-theorem.md) for [simply connected spaces](../../../../../../simply-connected-space.md) makes the map of [CW complex](../../../../../../cw-complex.md) models a homotopy equivalence. Returning to the original spaces therefore gives

$$
\boxed{f\text{ is a weak homotopy equivalence}.}
$$

The simply connected hypothesis is used both in the first-nonzero-degree [Hurewicz theorem](../../../../../../hurewicz-theorem.md) argument and in the final [homological Whitehead theorem](../../../../../../homological-whitehead-theorem.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
