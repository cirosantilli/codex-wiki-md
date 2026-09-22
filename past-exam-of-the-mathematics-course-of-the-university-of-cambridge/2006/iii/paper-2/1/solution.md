<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Suppose first that $M$ is a [Noetherian module](../../../../../noetherian-module.md). An ascending chain of [submodules](../../../../../submodule.md) of $N$ is also a chain in $M$, so it stabilizes. A chain in the [quotient module](../../../../../quotient-module.md) $M/N$ lifts to a chain in $M$, so it also stabilizes. Thus both $N$ and $M/N$ are [Noetherian modules](../../../../../noetherian-module.md).

Conversely, let $M_1\subseteq M_2\subseteq\cdots$ be a chain of [submodules](../../../../../submodule.md) of $M$. If $N$ and $M/N$ are [Noetherian modules](../../../../../noetherian-module.md), both $M_i\cap N$ and $(M_i+N)/N$ stabilize, say for $i\geq i_0$. For $x\in M_{i+1}$, equality of the images gives $y\in M_i$ with $x-y\in N$. Then $x-y\in M_{i+1}\cap N=M_i\cap N$, and hence $x\in M_i$. This proves the extension direction of [Noetherian modules in a short exact sequence](../../../../../noetherian-modules-in-a-short-exact-sequence.md).

The left regular [module](../../../../../module-mathematics.md) $R$ is [Noetherian](../../../../../noetherian-ring.md) because $R$ is a [left Noetherian ring](../../../../../left-noetherian-ring.md). Applying the extension result inductively makes each finite [direct sum](../../../../../direct-sum.md) $R^s$ [Noetherian](../../../../../noetherian-ring.md). Every [finitely generated module](../../../../../finitely-generated-module.md) on the left is a [quotient module](../../../../../quotient-module.md) of such a [direct sum](../../../../../direct-sum.md), so it is [Noetherian](../../../../../noetherian-ring.md).

A [poly-(cyclic or finite) group](../../../../../poly-cyclic-or-finite-group.md) has a finite [subnormal series](../../../../../subnormal-series.md)

$$
1=G_0\triangleleft G_1\triangleleft\cdots\triangleleft G_\ell=G
$$

whose factors are [cyclic groups](../../../../../cyclic-group.md) or [finite groups](../../../../../finite-group.md). We prove that the [group ring](../../../../../group-ring.md) $R[G_i]$ is a [left Noetherian ring](../../../../../left-noetherian-ring.md) by induction. Put $A=R[G_{i-1}]$. A finite factor makes $R[G_i]$ a finite free left $A$-[module](../../../../../module-mathematics.md), using a coset transversal. Its [left ideals](../../../../../left-ideal.md) are $A$-[submodules](../../../../../submodule.md), so [finite-module extension preserves Noetherianity](../../../../../finite-module-extension-preserves-noetherianity.md) handles this case.

If the factor is infinite cyclic, choose a lift $t$ of a generator and let $\sigma(a)=tat^{-1}$. The [group ring](../../../../../group-ring.md) is the [skew Laurent polynomial ring](../../../../../skew-laurent-polynomial-ring.md) $A[t,t^{-1};\sigma]$. Here is the required left-sided [skew Hilbert basis theorem](../../../../../skew-hilbert-basis-theorem.md). For a [left ideal](../../../../../left-ideal.md) $L\subseteq A[t;\sigma]$, define

$$
I_n=\left\{\sigma^{-n}(a_n):\sum_{j=0}^n a_jt^j\in L\right\}.
$$

Each $I_n$ is a [left ideal](../../../../../left-ideal.md) of $A$. Left multiplication by $t$ gives $I_n\subseteq I_{n+1}$. The [ascending chain condition](../../../../../ascending-chain-condition.md) makes these ideals constant for $n\geq n_0$; choose finitely many generators for each $I_n$, $0\leq n\leq n_0$, and lift them to polynomials $f_{nj}\in L$.

If $f\in L$ has degree $d\geq n_0$ and leading coefficient $a_d$, write

$$
\sigma^{-d}(a_d)=\sum_j r_j\sigma^{-n_0}(a_{n_0j}).
$$

Subtracting $\sum_j\sigma^d(r_j)t^{d-n_0}f_{n_0j}$ cancels the leading coefficient. For $d<n_0$, use the lifts for $I_d$ instead. Induction on [polynomial degree](../../../../../degree-of-a-polynomial.md) shows that the finitely many $f_{nj}$ generate $L$. Thus the [skew polynomial ring of an automorphism](../../../../../skew-polynomial-ring-of-an-automorphism.md) is a [left Noetherian ring](../../../../../left-noetherian-ring.md).

Finally, for a [left ideal](../../../../../left-ideal.md) $K$ of $A[t,t^{-1};\sigma]$, its intersection with $A[t;\sigma]$ has finitely many generators. Every $f\in K$ satisfies $t^mf\in A[t;\sigma]$ for some $m\geq0$, so those same generators generate $K$ after multiplication by $t^{-m}$. This completes the induction and proves that **$R[G]$ is left Noetherian**, the left-sided form of [group rings of poly-(cyclic or finite) groups are Noetherian](../../../../../group-rings-of-poly-cyclic-or-finite-groups-are-noetherian.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
