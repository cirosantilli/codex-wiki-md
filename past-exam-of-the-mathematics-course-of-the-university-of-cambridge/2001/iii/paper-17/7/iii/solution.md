<h1 id="7/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Only $L\Rightarrow A$ remains. Assume $U$ preserves small [categorical limits](../../../../../../categorical-limit.md), and choose a [small cogenerating family](../../../../../../cogenerating-set.md) $(Q_i)_{i\in I}$ in $\mathcal C$. Fix a [set](../../../../../../set-split.md) $X$. The [comma category](../../../../../../comma-category.md) $(X\downarrow U)$ is a [complete category](../../../../../../complete-category.md): underlying limits in $\mathcal C$, together with limit preservation by $U$, lift compatible maps from $X$. It is [locally small](../../../../../../locally-small-category.md), since its arrows form subsets of the [hom-sets](../../../../../../hom-set.md) in $\mathcal C$.

We construct a [weakly initial set](../../../../../../weakly-initial-set.md) in this comma category. Given $f:X\to U(C)$, intersect all [subobjects](../../../../../../subobject.md) $m:B\hookrightarrow C$ through which $f$ lifts under $U$. There are only a [set](../../../../../../set-split.md) of subobjects because $\mathcal C$ is [well-powered](../../../../../../well-powered-category.md); the family includes $1_C$. Their intersection exists by completeness. Also $U$ preserves [monomorphisms](../../../../../../monomorphism.md), since a map is monic precisely when its self-pullback diagonal is invertible, and $U$ preserves such [pullbacks](../../../../../../pullback-category-theory.md).

Thus all lifts of $f$ are unique and compatible, and preservation of the intersection gives

$$
f=U(m_0)f_0,\qquad m_0:C_0\hookrightarrow C.
$$

No proper [subobject](../../../../../../subobject.md) of $C_0$ supports a lift of $f_0$: its composite into $C$ would belong to the intersected family, forcing it to contain $C_0$. This is a [minimal supported subobject](../../../../../../minimal-supported-subobject.md).

For each $i$, the map

$$
\mathcal C(C_0,Q_i)\longrightarrow\mathbf{Set}(X,UQ_i),\qquad
h\longmapsto U(h)f_0
$$

is [injective](../../../../../../injective-function.md). Indeed, equal images mean $f_0$ lifts to the [equalizer](../../../../../../equaliser.md) of the two maps, because $U$ preserves that equalizer. Minimality forces the equalizer to be invertible, so the maps agree.

The [cogenerator](../../../../../../coseparator.md) property makes the evaluation map

$$
C_0\longrightarrow\prod_{i\in I,\ h:C_0\to Q_i}Q_i
$$

a [monomorphism](../../../../../../monomorphism.md): any two arrows into $C_0$ that agree after all these projections are equal. The indexing pairs $(i,h)$ inject into the fixed set

$$
B_X=\coprod_{i\in I}\mathbf{Set}(X,UQ_i).
$$

Their image is some subset $J\subseteq B_X$. Consequently $C_0$ is isomorphic to a [subobject](../../../../../../subobject.md) of a product $P_J$ of the $Q_i$ indexed by $J$. There are only a set of such subsets $J$, only a set of subobjects of each $P_J$, and only a set of maps $X\to U(B)$ for each representative subobject $B$.

Collect all these pairs $(B,x:X\to U(B))$. Every $(C,f)$ receives a comma arrow from one of them, via the isomorphic copy of $(C_0,f_0)$ and $m_0$. Hence they form a [weakly initial set](../../../../../../weakly-initial-set.md). The [initial-object lemma for complete categories with a weakly initial set](../../../../../../initial-object-lemma-for-complete-categories-with-a-weakly-initial-set.md), proved explicitly in Question 8, gives an initial object of $(X\downarrow U)$. Its map from $X$ is a [universal arrow from an object to a functor](../../../../../../universal-arrow-from-an-object-to-a-functor.md). Choosing these universal arrows for all $X$ defines a [left adjoint](../../../../../../adjoint-functors.md) to $U$.

Thus

$$
\boxed{A\Longleftrightarrow R\Longleftrightarrow L.}
$$

The products indexed by realized subsets $J$ are important: one cannot assume that $C_0$ has a map to every cogenerator and simply add arbitrary missing coordinates.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [7](../../7.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
