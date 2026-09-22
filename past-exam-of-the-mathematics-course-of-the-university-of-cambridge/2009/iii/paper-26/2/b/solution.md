<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At every good prime we have $p\ne2$. After removing any even p-adic valuation in the parameter as in part (a), use a smooth reduction $y^2=x^3-d^2x$ with $d\in\mathbb F_p^\times$. Let $\chi$ be the [Legendre symbol](../../../../../../legendre-symbol.md), extended by $\chi(0)=0$. Counting the two, one or zero y-values above each x gives

$$
\#\widetilde E_D(\mathbb F_p)=p+1+\sum_{x\in\mathbb F_p}\chi(x^3-d^2x),\qquad
a_p=-\sum_x\chi(x^3-d^2x).
$$

If $p\equiv3\pmod4$, then $\chi(-1)=-1$. The terms for $x$ and $-x$ cancel, including zeros, because the cubic is odd. Hence $a_p=0$.

For the converse, the four distinct points $O,(0,0),(d,0),(-d,0)$ form the full rational [2-torsion](../../../../../../2-torsion.md) subgroup of the reduced curve. Its group order is therefore divisible by four. If $p\equiv1\pmod4$, zero trace would give group order $p+1\equiv2\pmod4$, a contradiction. Consequently

$$
\boxed{a_p=0\iff p\equiv3\pmod4.}
$$

This is the [vanishing trace criterion for a congruent number curve](../../../../../../vanishing-trace-criterion-for-a-congruent-number-curve.md). The [Hasse theorem for elliptic curves](../../../../../../hasse-s-theorem-on-elliptic-curves.md) states

$$
\boxed{|a_p|\leq2\sqrt p.}
$$

For good primes that divide a nonsquarefree displayed parameter, the tilde denotes the smooth reduction of a minimal model, not the singular special fibre of that nonminimal equation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
