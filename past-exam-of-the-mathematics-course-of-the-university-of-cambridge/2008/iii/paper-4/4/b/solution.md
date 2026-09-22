<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the basis of $D$-conjugation orbit sums in $kG$. A singleton orbit is exactly an element of $C_G(D)$, so these basis vectors span the subring $kC_G(D)$. For a nonsingleton orbit with representative $x$, its stabilizer is the proper [subgroup](../../../../../../subgroup.md) $E=C_D(x)<D$, and its orbit sum is $\operatorname{Tr}_E^D(x)$. Thus every nonsingleton basis vector belongs to the sum of proper-subgroup transfer images.

Conversely the coefficient at a $D$-fixed basis element $x\in C_G(D)$ in $\operatorname{Tr}_E^D(a)$ is $[D:E]a_x=0$ in characteristic $p$ whenever $E<D$. Hence the two spans intersect trivially, giving

$$
\boxed{(kG)^D=kC_G(D)\oplus I_D^{\mathrm{prop}},\qquad
I_D^{\mathrm{prop}}=\sum_{E<D}\operatorname{Tr}_E^D((kG)^E).}
$$

For $u\in(kG)^D$, multiplication by a transfer element satisfies $u\operatorname{Tr}_E^D(a)=\operatorname{Tr}_E^D(ua)$ and $\operatorname{Tr}_E^D(a)u=\operatorname{Tr}_E^D(au)$. Therefore the second summand is a two-sided [ideal](../../../../../../ideal.md), as required; it need not be nilpotent in this general setting.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
