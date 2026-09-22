<h1 id="17g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose $\chi$ is an [irreducible character](../../../../../../irreducible-character.md) of a group of odd order and $\chi=\overline\chi$. Write $d=\chi(1)$. Every nonidentity element pairs with its distinct inverse, since there is no element of order $2$. Also $\chi(g^{-1})=\overline{\chi(g)}=\chi(g)$. If $\chi$ were nontrivial, [character orthogonality](../../../../../../character-orthogonality.md) with the trivial [character of a representation](../../../../../../character-of-a-representation.md) would give

$$
\langle\chi,1_G\rangle=\frac{d+2A}{|G|},\qquad 0=d+2A,
$$

where $A$ is the sum of one [character of a representation](../../../../../../character-of-a-representation.md) value from each inverse pair. This $A$ is an [algebraic integer](../../../../../../algebraic-integer.md), so $A=-d/2\in\mathbb Q$ is an [integer](../../../../../../integer.md). Hence $d$ is even.

But an [irreducible character degree divides the group order](../../../../../../irreducible-character-degree-divides-the-group-order.md), so $d$ must be odd. One quick justification of that divisibility is that the central class sum of a [conjugacy class](../../../../../../conjugacy-class.md) $C$ acts by the [algebraic integer](../../../../../../algebraic-integer.md) $\lambda_C=|C|\chi(g_C)/d$. Its integrality follows from its [integer](../../../../../../integer.md) [matrix](../../../../../../matrix.md) on the regular [group representation](../../../../../../group-representation.md). [Character orthogonality](../../../../../../character-orthogonality.md) then gives

$$
\frac{|G|}{d}=\sum_C\lambda_C\overline{\chi(g_C)},
$$

a rational [algebraic integer](../../../../../../algebraic-integer.md), hence an [integer](../../../../../../integer.md). The parity contradiction proves $\boxed{\chi=1_G}$: **the trivial character is the only self-conjugate [irreducible character](../../../../../../irreducible-character.md) of an odd-order group**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17G](../../17g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
