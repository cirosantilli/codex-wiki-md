<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

[Lagrange's theorem](../../../../../lagrange-s-theorem.md) states that for a [subgroup](../../../../../subgroup.md) $H$ of a finite [group](../../../../../group-split.md) $G$, $|G|=[G:H]|H|$; in particular $|H|$ divides $|G|$. This follows by partitioning $G$ into [cosets](../../../../../coset.md), each in [bijection](../../../../../bijection.md) with $H$.

If $|G|=p$ is prime, take any $g\ne e$. Its [cyclic subgroup](../../../../../cyclic-subgroup.md) has order dividing $p$, but its order is not one. Thus it has order $p$ and equals $G$. Hence

$$
\boxed{\text{Every group of order }p\text{ is cyclic and isomorphic to }C_p.}
$$

This describes a single [group isomorphism](../../../../../group-isomorphism.md) type for each prime.

Now let $G=\langle x\rangle$ have order $n$, and let $H$ be any [subgroup](../../../../../subgroup.md). Choose the least positive integer $d$ with $x^d\in H$; this exists because $x^n=e\in H$, even when $H$ is trivial. Divide $n=qd+r$ with $0\le r<d$. Since $x^r=x^n(x^d)^{-q}\in H$, minimality forces $r=0$, so $d$ divides $n$. Likewise, dividing an exponent $k=qd+r$ for any $x^k\in H$ shows $r=0$. Therefore $H=\langle x^d\rangle$.

Conversely, for each divisor $d$ of $n$, $\langle x^d\rangle$ is a [subgroup](../../../../../subgroup.md) of order $n/d$. The least positive exponent property makes $d$ unique. This proves the complete [subgroups and quotients of a cyclic group](../../../../../subgroups-and-quotients-of-a-cyclic-group.md) classification:

$$
\boxed{H=\langle x^d\rangle\ (d\mid n),\quad |H|=n/d;
\qquad H_m=\langle x^{n/m}\rangle\text{ is the unique subgroup of order }m\ (m\mid n).}
$$

The choices $d=n$ and $d=1$ include the trivial [subgroup](../../../../../subgroup.md) and the whole [group](../../../../../group-split.md).

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
