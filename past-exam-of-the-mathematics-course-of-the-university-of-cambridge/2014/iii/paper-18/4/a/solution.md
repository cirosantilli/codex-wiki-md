<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $F:\mathcal C\to\mathcal D$ and $G:\mathcal D\to\mathcal C$. The characterization concerns an [adjunction](../../../../../../adjoint-functors.md) with the specified [unit and counit of an adjunction](../../../../../../unit-and-counit-of-an-adjunction.md) $\eta$ and $\varepsilon$. Its [triangle identities for an adjunction](../../../../../../triangle-identities-for-an-adjunction.md) are

$$
\boxed{\varepsilon_{FA}F\eta_A=1_{FA},\qquad G\varepsilon_D\eta_{GD}=1_{GD}.}
$$

Assume these identities. Define the hom-set maps

$$
\Phi(h)=Gh\,\eta_A\quad(h:FA\to D),\qquad
\Psi(f)=\varepsilon_DFf\quad(f:A\to GD).
$$

Naturality of $\eta$ and $\varepsilon$ makes these maps natural in both objects. Naturality and the [triangle identities for an adjunction](../../../../../../triangle-identities-for-an-adjunction.md) give

$$
\begin{aligned}
\Psi\Phi(h)&=\varepsilon_DFGh\,F\eta_A
=h\varepsilon_{FA}F\eta_A=h,\\
\Phi\Psi(f)&=G\varepsilon_DGFf\,\eta_A
=G\varepsilon_D\eta_{GD}f=f.
\end{aligned}
$$

Thus they are inverse [bijections](../../../../../../bijection.md) and define $F\dashv G$.

Conversely, from the natural hom-set [bijections](../../../../../../bijection.md) of an [adjunction](../../../../../../adjoint-functors.md), define $\eta_A=\Phi(1_{FA})$ and $\varepsilon_D=\Phi^{-1}(1_{GD})$. Naturality gives the same formulas for $\Phi$ and $\Psi$ above. Applying $\Psi\Phi$ to $1_{FA}$ and $\Phi\Psi$ to $1_{GD}$ gives the two [triangle identities for an adjunction](../../../../../../triangle-identities-for-an-adjunction.md). Therefore these identities are exactly the compatibility conditions on the specified unit and counit. If the printed equivalence were read as mere existence of some adjunction, independently of the supplied transformations, its only-if direction would be false: on the category of [abelian groups](../../../../../../abelian-group.md), $F=G=1$ are adjoint, but choosing both transformations to be zero does not satisfy either triangle on a nonzero object.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
