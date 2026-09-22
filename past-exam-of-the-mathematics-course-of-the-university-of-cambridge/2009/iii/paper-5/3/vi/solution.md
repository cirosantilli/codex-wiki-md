<h1 id="3/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

Write $G=\langle a,b\rangle$ and $c=[a,b]$. The [commutator subgroup](../../../../../../commutator-subgroup.md) $G\prime$ is the [normal closure](../../../../../../normal-closure.md) of $c$: imposing $c=1$ makes the two generators commute, so the quotient is abelian. Part (iii), with $N=G$, makes $G\prime$ a [powerfully embedded subgroup](../../../../../../powerfully-embedded-subgroup.md). Part (ii) therefore gives

$$
G\prime=\langle c\rangle.
$$

This proves the hint, but cyclicity of the [commutator subgroup](../../../../../../commutator-subgroup.md) alone is not yet the required cyclic normal subgroup with cyclic quotient.

If $c=1$, the [group](../../../../../../group-split.md) is abelian and any one of the two generator subgroups is normal with cyclic quotient. Otherwise $c\in G^p$. Part (v) permits taking a $p$th root of $c$. Whenever the chosen root is still in $G^p$, take another $p$th root. The order increases by a factor $p$ at every step, since the power being rooted is nonidentity. Finiteness forces this process to stop. Thus

$$
c=d^{p^r},\qquad d\notin G^p=\Phi(G)
$$

for some $d$. The [cyclic subgroup](../../../../../../cyclic-subgroup.md) $A=\langle d\rangle$ contains $G\prime$, and hence is normal: every conjugate of $d$ differs from $d$ by an element of $G\prime\leq A$. The nonzero image of $d$ in the [Frattini quotient](../../../../../../frattini-quotient.md) can be completed to a basis of dimension at most two. By the [Burnside basis theorem](../../../../../../burnside-basis-theorem.md), $G=\langle d,e\rangle$ for a suitable $e$; if the quotient has dimension one, $d$ already generates $G$. Therefore $G/A$ is cyclic. **The powerful two-generator finite p-group is metacyclic.**

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [3](../../3.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
