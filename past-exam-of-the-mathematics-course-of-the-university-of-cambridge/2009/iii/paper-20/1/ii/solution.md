<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

There are no [one-handles](../../../../../../one-handle.md), so attaching the three [two-handles](../../../../../../two-handle.md) to a four-ball cannot create a [fundamental group](../../../../../../fundamental-group.md) generator: **$\pi_1(W)=1$**. The handle [chain complex](../../../../../../chain-complex.md) has $C_2=\mathbb Z^3$, $C_1=0$ and $C_0=\mathbb Z$, giving

$$
\boxed{H_0(W)=\mathbb Z,\qquad H_2(W)=\mathbb Z^3,\qquad H_j(W)=0\ (j\ne0,2).}
$$

To calculate the boundary, orient the two long components down their central strands, and orient the small component clockwise. The six mutual crossings of the long components have negative sign, giving [linking number](../../../../../../linking-number.md) $-3$. Each long component has two positive crossings with the small component, giving [linking number](../../../../../../linking-number.md) $1$. The [surgery linking matrix](../../../../../../surgery-linking-matrix.md), in the order of framings $4,3,2$, is consequently

$$
Q=\begin{pmatrix}4&-3&1\\-3&3&1\\1&1&2\end{pmatrix},\qquad\det Q=-7.
$$

Changing a component orientation changes the corresponding row and column signs, and does not change the resulting [homology](../../../../../../homology-split.md). The [long exact sequence of a pair](../../../../../../long-exact-sequence-in-relative-homology.md) and [Poincare-Lefschetz duality](../../../../../../lefschetz-duality.md) identify $H_2(\partial W)=\ker Q$ and $H_1(\partial W)=\operatorname{coker}Q$. The determinant is nonzero, so the kernel vanishes. The gcd of matrix entries is one; the two-by-two minors include $-6$ and $7$, so their gcd is also one. The [Smith normal form](../../../../../../smith-normal-form.md) therefore has diagonal $1,1,7$, and

$$
\boxed{H_j(\partial W;\mathbb Z)=\begin{cases}\mathbb Z,&j=0,3,\\\mathbb Z/7,&j=1,\\0,&j=2\text{ or }j\ge4.\end{cases}}
$$

In particular the sign of the braid crossings matters: replacing $-3$ by $+3$ while leaving both meridian linkings positive would represent a different link and would give the wrong determinant.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
