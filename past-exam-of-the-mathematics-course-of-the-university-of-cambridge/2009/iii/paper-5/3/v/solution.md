<h1 id="3/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Set $P_0=G$ and $P_{i+1}=P_i^p$. The permitted power-embedding result, applied repeatedly, gives $[P_i,G]\leq P_{i+1}$, and each $P_i$ is a [powerful p-group](../../../../../../powerful-p-group.md). These [subgroups](../../../../../../subgroup.md) eventually reach $1$: if $P_i\ne1$, its [Frattini subgroup](../../../../../../frattini-subgroup.md) $P_i^p$ is proper. In fact these are the [lower p-series](../../../../../../lower-p-series.md) layers, with their indices shifted by one.

For $x\in G$ and $y\in P_i$, the [commutator](../../../../../../commutator.md) $[y,x]$ lies in $P_{i+1}$, is central modulo $P_{i+2}$, and has exponent dividing $p$ there. The class-two collection calculation from part (iv) therefore gives

$$
(xy)^p\equiv x^py^p\pmod {P_{i+2}}.
$$

Applying part (iv) inside $P_i$, whose third lower-series term is contained in $P_{i+2}$, shows that the map $y\mapsto y^p$ is onto $P_{i+1}/P_{i+2}$.

Given $a\in P_1$, first choose $x$ with $x^p\equiv a\pmod {P_2}$. Suppose $x^p\equiv a\pmod {P_{i+1}}$. Choose $y\in P_i$ with $y^p\equiv x^{-p}a\pmod {P_{i+2}}$. The displayed collection congruence then gives $(xy)^p\equiv a\pmod {P_{i+2}}$. Replacing $x$ by $xy$ improves the approximation by one layer. Since the [filtration on a group](../../../../../../filtration-on-a-group.md) terminates, a finite sequence of corrections gives $x^p=a$ exactly. The reverse inclusion is the definition of $G^p$. Hence

$$
\boxed{G^p=G^{\{p\}}=\{x^p:x\in G\}.}
$$

## ↑ Ancestors (11)

1. [V](../v.md)
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
