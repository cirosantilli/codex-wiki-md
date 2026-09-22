<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $K:\mathcal B\to\mathcal C$, $J:\mathcal C\to\mathcal B$, with [adjunction unit](../../../../../../unit-of-an-adjunction.md) $\rho$ and [adjunction counit](../../../../../../counit-of-an-adjunction.md) $\varepsilon$. The [adjunction](../../../../../../adjoint-functors.md) gives

$$
\mathcal C(KJC,C')\cong\mathcal B(JC,JC'),\qquad h\longmapsto J(h)\rho_{JC}.
$$

For $f:C\to C'$, precomposition with $\varepsilon_C$ followed by this [bijection](../../../../../../bijection.md) gives

$$
J(f\varepsilon_C)\rho_{JC}=Jf,
$$

by the [triangle identities for an adjunction](../../../../../../triangle-identities-for-an-adjunction.md). Thus $J$ is [fully faithful](../../../../../../full-and-faithful-functor.md) exactly when precomposition with $\varepsilon_C$ is bijective for every $C,C'$.

A [morphism](../../../../../../morphism.md) $e:P\to Q$ with this property is an [isomorphism](../../../../../../isomorphism.md). Surjectivity for target $P$ supplies $u:Q\to P$ with $ue=1_P$. Since $(eu)e=e=1_Qe$, injectivity for target $Q$ gives $eu=1_Q$. Conversely, precomposition with an [isomorphism](../../../../../../isomorphism.md) is always bijective. Applied to every $\varepsilon_C$, this proves **the fully faithful right-adjoint criterion**:

$$
\boxed{J\text{ is fully faithful}\iff\varepsilon:KJ\Rightarrow1_{\mathcal C}\text{ is a natural isomorphism}.}
$$

When the [adjunction counit](../../../../../../counit-of-an-adjunction.md) is invertible, the inverse to $f\mapsto Jf$ is explicitly $h\mapsto\varepsilon_{C'}K(h)\varepsilon_C^{-1}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
