<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

An [integral scheme](../../../../../integral-scheme.md) is nonempty, reduced and irreducible. For an [affine scheme](../../../../../affine-scheme.md) $X=\operatorname{Spec}R$, reducedness is equivalent to $\sqrt{(0)}=0$: [nilpotent elements](../../../../../nilpotent.md) vanish in every [stalk](../../../../../stalk-of-a-sheaf.md), and conversely a nonzero element has nonzero [localization](../../../../../localization-of-a-ring.md) somewhere. Irreducibility is equivalent to the [nilradical](../../../../../nilradical.md) being prime. Indeed, if $ab$ lies in every prime, then $V(ab)=V(a)\cup V(b)=X$; irreducibility makes one of these closed subsets all of $X$, so $a$ or $b$ lies in the [nilradical](../../../../../nilradical.md). Conversely, if the [nilradical](../../../../../nilradical.md) is prime, its point is a [generic point](../../../../../generic-point.md) of the whole spectrum. Thus reducedness and irreducibility together say that zero is a [prime ideal](../../../../../prime-ideal.md), with $R\ne0$. Therefore

$$
\boxed{\operatorname{Spec}R\text{ is integral}\iff R\text{ is an integral domain}.}
$$

For a global [idempotent](../../../../../idempotent.md) $e$, its germ in any [local ring](../../../../../local-ring.md) is either zero or one. To see this, $e(1-e)=0$, and at least one of $e,1-e$ is a unit. Multiplication by that unit forces the other to vanish. On each [affine chart](../../../../../affine-chart-of-a-variety.md),

$$
\boxed{V(1-e)=D(e),\qquad X\setminus V(1-e)=V(e)=D(1-e).}
$$

These equalities also hold globally. Hence $V(1-e)$ is a [clopen set](../../../../../clopen-set.md). Conversely, on a [clopen](../../../../../clopen-set.md) subset $U$ and its complement, glue the sections one and zero. They define a global [idempotent](../../../../../idempotent.md) $e_U$, and the two constructions are inverse. This proves the [idempotent–clopen correspondence](../../../../../idempotent-clopen-correspondence.md).

Assume each [connected component](../../../../../connected-component.md) is open. Every [clopen](../../../../../clopen-set.md) subset is a union of [connected components](../../../../../connected-component.md), since its intersection with a [connected component](../../../../../connected-component.md) is [clopen](../../../../../clopen-set.md) in that component. Each individual component is also closed, so it defines a nonzero [idempotent](../../../../../idempotent.md). A decomposition into two nonempty disjoint [clopen](../../../../../clopen-set.md) subsets corresponds exactly to a sum of two nonzero [orthogonal idempotents](../../../../../orthogonal-idempotent.md). A union containing at least two components admits such a decomposition by separating one component from the rest. A single component admits none. Consequently the precise conclusion is

$$
\boxed{\{\text{connected components of }X\}\ \longleftrightarrow\ \{\text{primitive idempotents of }\Gamma(X,\mathcal O_X)\}.}
$$

The printed definition needs both **nonzero** and **orthogonal**. Literally forbidding every sum of two nonzero [idempotents](../../../../../idempotent.md) gives a false statement in characteristic two. For $X=\operatorname{Spec}(\mathbb F_2\times\mathbb F_2)$, the component [idempotent](../../../../../idempotent.md) $(1,0)$ decomposes as $(1,1)+(0,1)$; both summands are nonzero [idempotents](../../../../../idempotent.md) but are not orthogonal. In fact each of the three nonzero [idempotents](../../../../../idempotent.md) in this [ring](../../../../../ring.md) decomposes into the other two, although $X$ has two open [connected components](../../../../../connected-component.md). Excluding zero is also necessary: zero corresponds to the empty subset, not to a component. With the standard [primitive idempotent](../../../../../primitive-idempotent.md) definition the preceding proof establishes the intended bijection in every characteristic.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 89](../../paper-89-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
