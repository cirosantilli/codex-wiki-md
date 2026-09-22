<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

A [BQO](../../../../../better-quasi-ordering.md), or [better-quasi-ordering](../../../../../better-quasi-ordering.md), strengthens a [well-quasi-ordering](../../../../../well-quasi-ordering.md) by testing arrays indexed by arbitrary barriers, rather than just [sequences](../../../../../sequence.md). Let $Q$ be a [preorder](../../../../../preorder.md). A [barrier in better-quasi-order theory](../../../../../barrier-in-better-quasi-order-theory.md) on an infinite $A\subseteq\omega$ is a family $B$ of nonempty finite increasing [sequences](../../../../../sequence.md) such that no member is properly contained in another and every infinite [subset](../../../../../subset.md) of $A$ has a member of $B$ as its initial segment.

For barrier members write $s\triangleleft t$ if a finite increasing [sequence](../../../../../sequence.md) $u$ has $s$ as an initial segment and has $t$ as an initial segment after deleting the first entry of $u$. A map $f:B\to Q$ is good when some $s\triangleleft t$ satisfy $f(s)\leq f(t)$. The definition is

$$
\boxed{Q\text{ is BQO }\Longleftrightarrow
\text{ every map from every barrier into }Q\text{ is good}.}
$$

Both quantifiers matter: testing only barriers of one fixed finite length is insufficient.

For the singleton barrier $B=[A]^1$, shifted pairs are just $\{a\}\triangleleft\{b\}$ with $a<b$. Thus the BQO condition implies the ordinary [well-quasi-ordering](../../../../../well-quasi-ordering.md) condition. Barrier arrays can also be viewed through [continuous arrays in better-quasi-order theory](../../../../../continuous-array-in-better-quasi-order-theory.md) $F:[A]^\omega\to Q$, with $Q$ discrete: [set](../../../../../set-split.md) $F(X)=f(s)$ for the unique barrier initial segment $s$ of $X$. This is continuous because that value is fixed by a finite prefix, and comparing $X$ with $X\setminus\{\min X\}$ is exactly the shift comparison. The general continuous-array formulation is equivalent to the barrier definition; its converse uses refinement of fronts to barriers, rather than the incorrect assertion that every prefix-decision family is already a barrier.

For an illustrative positive example, every [well-order](../../../../../well-order.md) is a BQO. If a barrier array into a [well-order](../../../../../well-order.md) were bad, its induced $F$ would satisfy

$$
F(X)>F(X\setminus\{\min X\})
>F(X\setminus\{\text{first two entries}\})>\cdots
$$

for every infinite $X$. This is an infinite strict descent in a [well-order](../../../../../well-order.md), a contradiction. A finite antichain with equality is also a BQO: the finitely many fibres of the induced continuous array are [open](../../../../../open-set.md), so repeated use of the [Open Ramsey theorem](../../../../../open-ramsey-theorem.md) gives an infinite $A'$ on which the array is constant. The comparison of an infinite [subset](../../../../../subset.md) of $A'$ with its shift is then good.

The implication to a well-quasi-order is strict. The [Rado order](../../../../../rado-order.md) is

$$
R=\{(m,n)\in\omega^2:m<n\},\qquad
(m,n)\leq_R(k,l)\ \Longleftrightarrow\
(m=k\text{ and }n\leq l)\text{ or }n<k.
$$

It is [well-quasi-ordered](../../../../../well-quasi-ordering.md): if one first coordinate occurs infinitely often, its second coordinates have an increasing pair; otherwise the first coordinates are unbounded, and a later one exceeds the second coordinate of a chosen earlier pair. But take the barrier $[\omega]^2$ and $f(\{m,n\})=(m,n)$. For $m<n<l$, the shift compares $(m,n)$ with $(n,l)$; their first coordinates differ and $n<n$ is false. Every shifted comparison therefore fails. This [bad barrier array for the Rado order](../../../../../bad-barrier-array-for-the-rado-order.md) proves **[well-quasi-ordering](../../../../../well-quasi-ordering.md) does not imply [better-quasi-ordering](../../../../../better-quasi-ordering.md)**.

The stronger notion is designed for infinitary closure operations, such as powerset and infinite-sequence constructions, where a mere well-quasi-order can develop new bad arrays. The barrier definition records variable finite amounts of information from an infinite object and is consequently more robust than checking [sequences](../../../../../sequence.md) alone.

## ↑ Ancestors (10)

1. [8](../8.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
