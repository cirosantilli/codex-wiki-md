<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**Failure in general.** Let $f:\mathbb A^1_k=\operatorname{Spec}k[t]\to\operatorname{Spec}k$ be the [structure morphism](../../../../structure-morphism.md) and take the trivial [line bundle](../../../../line-bundle.md) $\mathcal L=\mathcal O_{\mathbb A^1_k}$. The [polynomial ring](../../../../polynomial-ring.md) $k[t]$ is a [Noetherian ring](../../../../noetherian-ring.md), so this is a [coherent sheaf](../../../../coherent-sheaf.md). Its [direct image](../../../../direct-image-sheaf.md) on the one-point target has sections

$$
\Gamma(\operatorname{Spec}k,f_*\mathcal L)=k[t].
$$

A [coherent sheaf](../../../../coherent-sheaf.md) on $\operatorname{Spec}k$ corresponds to a finite-dimensional [vector space](../../../../vector-space-split.md) over $k$, whereas $1,t,t^2,\ldots$ are [linearly independent](../../../../linear-independence.md). Thus

$$
\boxed{f_*\mathcal O_{\mathbb A^1_k}\text{ is not coherent}.}
$$

**Quasi-coherence for the stated morphism.** Now let $f$ satisfy (a), and let $\mathcal F$ be a [quasi-coherent sheaf](../../../../quasi-coherent-sheaf.md) on $X$. Over any [affine open subscheme](../../../../affine-open-subscheme.md) $V=\operatorname{Spec}A$ of $Y$, write $f^{-1}V=\operatorname{Spec}B$ and $\mathcal F|_{f^{-1}V}=\widetilde M$ for a $B$-[module](../../../../module-mathematics.md) $M$. Regard $M$ as an $A$-[module](../../../../module-mathematics.md) through the [ring homomorphism](../../../../ring-homomorphism.md) $A\to B$. For $a\in A$,

$$
\Gamma(D(a),f_*\mathcal F)
=\Gamma\bigl(D(\varphi(a)),\widetilde M\bigr)
=M_{\varphi(a)}=M_a.
$$

The last two [localizations](../../../../localization-of-a-ring.md) are identical: both invert the action of the same element on $M$. These identifications commute with restrictions, so on the basis of [principal open subsets](../../../../principal-open-subscheme.md) they identify $(f_*\mathcal F)|_V$ with the [affine module sheaf](../../../../affine-module-sheaf.md) $\widetilde{{}_AM}$. Hence this [direct image](../../../../direct-image-sheaf.md) is a [quasi-coherent sheaf](../../../../quasi-coherent-sheaf.md) on each $V$, and therefore on $Y$. This part uses only that $f$ is an [affine morphism](../../../../affine-morphism.md).

**Coherence under the Noetherian hypotheses.** If $X,Y$ are [Noetherian schemes](../../../../noetherian-scheme.md) and $\mathcal F$ is a [coherent sheaf](../../../../coherent-sheaf.md), then $M$ is a [finitely generated module](../../../../finitely-generated-module.md) over $B$. Choose generators $m_1,\ldots,m_s$ of $M$ over $B$, and generators $b_1,\ldots,b_r$ of $B$ over $A$, supplied by (a). Then the finite family

$$
\{b_jm_\ell:1\leq j\leq r,\ 1\leq\ell\leq s\}
$$

generates $M$ as an $A$-[module](../../../../module-mathematics.md): expand each coefficient of an expression $m=\sum_\ell c_\ell m_\ell$ in the $b_j$. Since $A$ is a [Noetherian ring](../../../../noetherian-ring.md), the [affine module sheaf](../../../../affine-module-sheaf.md) $\widetilde{{}_AM}$ is a [coherent sheaf](../../../../coherent-sheaf.md). This holds on an [affine open cover](../../../../affine-open-cover.md) of $Y$, proving

$$
\boxed{f_*:\operatorname{QCoh}(X)\to\operatorname{QCoh}(Y),\qquad
f_*:\operatorname{Coh}(X)\to\operatorname{Coh}(Y)\text{ if }X,Y\text{ are Noetherian}.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the introduction to schemes course of the University of Oxford](../../../split.md)
5. [Introduction to schemes course of the University of Oxford](../../../../introduction-to-schemes-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
