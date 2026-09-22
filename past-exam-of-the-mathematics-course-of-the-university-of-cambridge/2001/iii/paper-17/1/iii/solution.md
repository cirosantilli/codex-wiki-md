<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Define maps between the [hom-sets](../../../../../../hom-set.md) by

$$
\Phi(f)=G(f)\eta_A,\qquad \Psi(g)=\varepsilon_BF(g).
$$

Using [naturality](../../../../../../naturality.md) of the proposed [counit of an adjunction](../../../../../../counit-of-an-adjunction.md) and then the first [triangle identity for an adjunction](../../../../../../triangle-identities-for-an-adjunction.md),

$$
\Psi\Phi(f)=\varepsilon_BFG(f)F(\eta_A)
=f\varepsilon_{FA}F(\eta_A)=f.
$$

Using [naturality](../../../../../../naturality.md) of the proposed [unit of an adjunction](../../../../../../unit-of-an-adjunction.md) and then the other [triangle identity for an adjunction](../../../../../../triangle-identities-for-an-adjunction.md),

$$
\Phi\Psi(g)=G(\varepsilon_B)GF(g)\eta_A
=G(\varepsilon_B)\eta_{GB}g=g.
$$

Hence $\Phi$ and $\Psi$ are inverse [bijections](../../../../../../bijection.md). They are natural in both variables: for $a:A'\to A$ and $b:B\to B'$, the [unit of an adjunction](../../../../../../unit-of-an-adjunction.md) identity gives

$$
\Phi(bfF(a))=G(b)G(f)GF(a)\eta_{A'}
=G(b)\Phi(f)a.
$$

This constructs an [adjunction](../../../../../../adjoint-functors.md) $F\dashv G$. Taking $f=1_{FA}$ and $g=1_{GB}$ recovers the prescribed [unit of an adjunction](../../../../../../unit-of-an-adjunction.md) and [counit of an adjunction](../../../../../../counit-of-an-adjunction.md). Conversely, part (i) shows that any [adjunction](../../../../../../adjoint-functors.md) with those components must have exactly these transpose formulas. **The adjunction exists and is unique with the prescribed unit and counit.**

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
