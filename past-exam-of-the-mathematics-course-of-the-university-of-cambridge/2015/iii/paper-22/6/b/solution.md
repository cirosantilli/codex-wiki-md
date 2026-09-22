<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $F:\mathcal X\to\mathcal A$ and $G:\mathcal A\to\mathcal X$, with [adjunction counit](../../../../../../counit-of-an-adjunction.md) $\varepsilon$. The induced [monad](../../../../../../monad.md) has $T=GF$ and $\mu=G\varepsilon F$. Define the [Eilenberg-Moore comparison functor](../../../../../../eilenberg-moore-comparison-functor.md) by

$$
\boxed{K(A)=(GA,G\varepsilon_A),\qquad K(f)=Gf.}
$$

The action $a_A=G\varepsilon_A:TGA\to GA$ satisfies $a_A\eta_{GA}=1_{GA}$ by a triangular equation. [Naturality](../../../../../../naturality.md) of $\varepsilon$ at $\varepsilon_A:FGA\to A$ gives

$$
\varepsilon_A FG\varepsilon_A=\varepsilon_A\varepsilon_{FGA}.
$$

Applying $G$ yields $a_A T(a_A)=a_A\mu_{GA}$, the other algebra identity. For $f:A\to A'$, [naturality](../../../../../../naturality.md) gives

$$
Gf\,G\varepsilon_A=G\varepsilon_{A'}\,GF(Gf),
$$

so $Gf$ is a [monad algebra morphism](../../../../../../morphism-of-algebras-for-a-monad.md). Identities and compositions are respected because $G$ is a [functor](../../../../../../functor.md). Finally,

$$
G^{\mathbb T}K(A)=GA,\qquad
KF(X)=(GFX,G\varepsilon_{FX})=(TX,\mu_X)=F^{\mathbb T}X,
$$

and the same equalities hold on [morphisms](../../../../../../morphism.md). Thus **both comparison identities hold**, strictly when $\mathbb T$ is the specified induced [monad](../../../../../../monad.md):

$$
\boxed{G^{\mathbb T}K=G,\qquad KF=F^{\mathbb T}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
