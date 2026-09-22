<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an invertible [braiding](../../../../../../braiding.md) $C$ satisfying the braid equation on $V\otimes V$, begin with the free associative [algebra over a field](../../../../../../algebra-over-a-field.md) on matrix coefficients $t_{ij}$, with $\Delta t_{ij}=\sum_kt_{ik}\otimes t_{kj}$ and $\varepsilon(t_{ij})=\delta_{ij}$. Impose precisely the coefficients of

$$
\delta_{V\otimes V}C=(C\otimes1)\delta_{V\otimes V},\qquad
\delta(e_i)=\sum_j e_j\otimes t_{ji}.
$$

This quotient is the [FRT bialgebra](../../../../../../frt-bialgebra.md), or [Faddeev-Reshetikhin-Takhtajan construction](../../../../../../rtt-construction.md). The relations form a [coideal](../../../../../../coideal.md) because composing two [coactions](../../../../../../coaction.md) that preserve $C$ again preserves $C$; the trivial [coaction](../../../../../../coaction.md) also preserves it, so the [counit](../../../../../../counit.md) descends. Universality follows because any such [coaction](../../../../../../coaction.md) must satisfy exactly these coefficient relations.

For the given $C$, take $t_{11}=a$, $t_{12}=b$, $t_{21}=c$, $t_{22}=d$. Thus $\delta(e_1)=e_1\otimes a+e_2\otimes c$ and $\delta(e_2)=e_1\otimes b+e_2\otimes d$. The coefficient relations, after cancellation of $q^{-1/2}$, are

$$
\boxed{ba=qab,\ ca=qac,\ db=qbd,\ dc=qcd,\ bc=cb,\ da-ad=(q-q^{-1})bc.}
$$

These are exactly the defining relations of $M_q(2)$ in the inverse-parameter convention of Question 1, without setting the [quantum determinant](../../../../../../quantum-determinant.md) equal to one. They therefore define mutually inverse [algebra homomorphisms](../../../../../../algebra-homomorphism-over-a-field.md): each named generator maps to the corresponding $t_{ij}$, and conversely. The matrix [comultiplication](../../../../../../comultiplication.md) and [counit](../../../../../../counit.md) are the same, so the isomorphism is also one of [bialgebras](../../../../../../bialgebra.md).

Here is the requested check of $ba=qab$ directly from $C$. Apply colinearity to $e_1\otimes e_2$ and compare the coefficient of $e_1\otimes e_1$. On the left, $C(e_1\otimes e_2)=q^{-1/2}e_2\otimes e_1$, giving $q^{-1/2}ba$. On the right, the corresponding term of $\delta(e_1\otimes e_2)$ is $e_1\otimes e_1\otimes ab$, and $C(e_1\otimes e_1)=q^{1/2}e_1\otimes e_1$. Hence $q^{-1/2}ba=q^{1/2}ab$, proving the relation. The other coefficient comparisons give the remaining displayed relations; no additional determinant relation is imposed in an [FRT bialgebra](../../../../../../frt-bialgebra.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
