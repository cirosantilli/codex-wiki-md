<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the usual convention that a [variety](../../../../../../algebraic-variety.md) is an [irreducible variety](../../../../../../irreducible-variety.md). For a [quasi-projective algebraic set](../../../../../../quasi-projective-algebraic-set.md) $T$, its [algebraic dimension](../../../../../../dimension-of-an-algebraic-set.md) is the supremum of the lengths $r$ of strict chains

$$
T_0\subsetneq T_1\subsetneq\cdots\subsetneq T_r
$$

of nonempty [irreducible closed subsets](../../../../../../irreducible-closed-subset.md) of $T$. It is the maximum of the [algebraic dimensions](../../../../../../dimension-of-an-algebraic-set.md) of its [irreducible components](../../../../../../irreducible-component.md). On an [affine algebraic set](../../../../../../affine-algebraic-set.md), the correspondence between [irreducible closed subsets](../../../../../../irreducible-closed-subset.md) and [prime ideals](../../../../../../prime-ideal.md) reverses inclusion, so this is the [Krull dimension](../../../../../../krull-dimension.md) of the [coordinate ring](../../../../../../coordinate-ring.md). On a [quasi-projective algebraic set](../../../../../../quasi-projective-algebraic-set.md), it is the supremum of the [Krull dimensions](../../../../../../krull-dimension.md) of the [coordinate rings](../../../../../../coordinate-ring.md) of its [affine open subsets](../../../../../../affine-open-subscheme.md). At a [closed point](../../../../../../closed-point.md) $x$, the [Krull dimension](../../../../../../krull-dimension.md) of the [local ring](../../../../../../local-ring.md) measures chains through $x$.

Here is a [closed-point dimension lemma for affine domains](../../../../../../closed-point-dimension-lemma-for-affine-domains.md) that avoids [transcendence degree](../../../../../../transcendence-degree.md). Put $A=k[X]$. By [Noether normalization](../../../../../../noether-normalization.md), there is a [integral extension](../../../../../../integral-extension.md)

$$
B=k[z_1,\ldots,z_d]\subset A.
$$

The number of variables is $d$ because [integral extensions preserve Krull dimension](../../../../../../integral-extensions-preserve-krull-dimension.md) and $\dim B=d$. For any [maximal ideal](../../../../../../maximal-ideal.md) $\mathfrak m$ of $A$, its contraction $\mathfrak n$ to $B$ is a [maximal ideal](../../../../../../maximal-ideal.md). Since $k$ is an [algebraically closed field](../../../../../../algebraically-closed-field.md), $\mathfrak n=(z_1-c_1,\ldots,z_d-c_d)$ has [height of a prime ideal](../../../../../../height-of-a-prime-ideal.md) $d$. The [going-down theorem](../../../../../../going-down-theorem.md) applies because $B$ is an [integrally closed domain](../../../../../../integrally-closed-domain.md) and $A$ is a [integral domain](../../../../../../integral-domain.md). It lifts a length-$d$ chain below $\mathfrak n$ to one below $\mathfrak m$. Hence

$$
\boxed{\dim A_{\mathfrak m}=\operatorname{ht}\mathfrak m=d.}
$$

The opposite inequality follows from $\dim A=d$.

For the nonempty [open subset](../../../../../../open-set.md) $U$, choose a nonempty [principal open subset](../../../../../../principal-open-subscheme.md) $D(g)\subset U$ and a [closed point](../../../../../../closed-point.md) $x\in D(g)$. Every [prime ideal](../../../../../../prime-ideal.md) below $\mathfrak m_x$ avoids $g$, so the preceding chain survives in the [localization](../../../../../../localization-of-a-ring.md) $A_g$. Consequently $\dim D(g)\ge d$. Conversely, any chain of [irreducible closed subsets](../../../../../../irreducible-closed-subset.md) in $U$ gives a chain of the same length after taking closures in $X$: intersecting those closures with $U$ recovers the original subsets. Therefore

$$
\boxed{\dim U=\dim X=d.}
$$

For the [principal hypersurface dimension lemma](../../../../../../principal-hypersurface-dimension-lemma.md), let $P$ be a [minimal prime ideal](../../../../../../minimal-prime-ideal.md) over $(f)$. Since $f\ne0$ in the [integral domain](../../../../../../integral-domain.md) $A$, $P\ne(0)$. The [Krull principal ideal theorem](../../../../../../krull-principal-ideal-theorem.md) gives $\operatorname{ht}P=1$. Choose a [closed point](../../../../../../closed-point.md) $x$ on $V(P)$ lying on none of the other finitely many [irreducible components](../../../../../../irreducible-component.md) of $V(f)$. Such a point exists because those other components cut out proper [closed subsets](../../../../../../closed-set.md) of the [irreducible variety](../../../../../../irreducible-variety.md) $V(P)$, and [closed points](../../../../../../closed-point.md) are dense. Set $R=A_{\mathfrak m_x}$. Then $\dim R=d$ and

$$
\sqrt{fR}=PR.
$$

Write $s=\dim R/fR$. Choose a [system of parameters](../../../../../../system-of-parameters.md) $\bar y_1,\ldots,\bar y_s$ in $R/fR$ and lift it to $R$. The [ideal](../../../../../../ideal.md) $(f,y_1,\ldots,y_s)$ has radical equal to the [maximal ideal](../../../../../../maximal-ideal.md) of $R$. The [Krull height theorem](../../../../../../krull-height-theorem.md) yields $d\le s+1$. On the other hand, any chain of [prime ideals](../../../../../../prime-ideal.md) containing $f$ can be extended strictly at the bottom by the zero [prime ideal](../../../../../../prime-ideal.md) of the [integral domain](../../../../../../integral-domain.md) $R$, giving $s\le d-1$. Thus $s=d-1$. Since $R/PR$ is a [localization](../../../../../../localization-of-a-ring.md) of $A/P$, $\dim A/P\ge d-1$. Extending a chain in $A/P$ by $(0)\subsetneq P$ also gives $\dim A/P\le d-1$. Hence **every component has the required dimension**:

$$
\boxed{\dim V(P)=d-1.}
$$

This argument uses [Noether normalization](../../../../../../noether-normalization.md), [going-down theorem](../../../../../../going-down-theorem.md), and the [Krull height theorem](../../../../../../krull-height-theorem.md), never the [dimension from the function field](../../../../../../dimension-from-the-function-field.md) theorem. Irreducibility is essential: if the word [variety](../../../../../../algebraic-variety.md) were instead allowed to mean an arbitrary reducible [affine algebraic set](../../../../../../affine-algebraic-set.md), neither assertion would hold without extra hypotheses. For example, a disjoint union of an [affine plane](../../../../../../affine-plane.md) and an [affine line](../../../../../../affine-line.md) has an open component of smaller [algebraic dimension](../../../../../../dimension-of-an-algebraic-set.md); a function equal to $1$ on the plane and a coordinate on the line has a nonempty zero set of [algebraic dimension](../../../../../../dimension-of-an-algebraic-set.md) $0$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
