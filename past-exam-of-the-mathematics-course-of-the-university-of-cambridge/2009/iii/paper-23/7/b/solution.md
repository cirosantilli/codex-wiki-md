<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the [adjunction unit](../../../../../../unit-of-an-adjunction.md) as $\eta:1_{\mathcal C}\Rightarrow GF$ and the [adjunction counit](../../../../../../counit-of-an-adjunction.md) as $\varepsilon:FG\Rightarrow1_{\mathcal D}$. Define the [monad induced by an adjunction](../../../../../../monad-induced-by-an-adjunction.md) by

$$
\boxed{T=GF,\qquad \mu_A=G\varepsilon_{FA}:GFGFA\to GFA,}
$$

with unit $\eta$. [Naturality](../../../../../../naturality.md) of $\varepsilon$ makes $\mu$ a [natural transformation](../../../../../../natural-transformation.md).

The [triangle identities for an adjunction](../../../../../../triangle-identities-for-an-adjunction.md) give the two unit laws:

$$
\mu_A\eta_{TA}=G\varepsilon_{FA}\eta_{GFA}=1_{GFA},\qquad
\mu_A T\eta_A=G(\varepsilon_{FA}F\eta_A)=1_{GFA}.
$$

For associativity, apply [naturality](../../../../../../naturality.md) of $\varepsilon$ to the arrow $\varepsilon_{FA}:FGFA\to FA$ in $\mathcal D$:

$$
\varepsilon_{FA}FG\varepsilon_{FA}=\varepsilon_{FA}\varepsilon_{FGFA}.
$$

Applying $G$ yields

$$
\mu_A T\mu_A=\mu_A\mu_{TA}.
$$

Thus the induced data satisfy all the [monad](../../../../../../monad.md) laws, rather than merely supplying an [endofunctor](../../../../../../endofunctor.md) and two transformations.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7](../../7.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
